---
name: LogMeIn
x-slug: logmein
description: LogMeIn, Inc. is a provider of software as a service and cloud-based
  remote connectivity services for collaboration, IT management and customer engagement,
  founded in 2003 and based in Boston, Massachusetts.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
x-kinRank: "7"
x-alexaRank: "7271"
tags: Transcripts
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/apis.md
specificationVersion: "0.14"
apis:
- name: GoToAssist Remote Support - Transcode Recordings
  x-api-slug: archiverecordingstranscodereadyfortranscoderecordingids-post
  description: "This method requests that a list of recordings be transcoded; once
    the API passes successfully, transcoding will be initiated for each of the recordings
    in the list. A result of \u201C204\u201D will be returned, regardless of the current
    state of the recordings (i.e., even if they are already transcoded). No more than
    500 recordings can be transcoded at once.\n\nNote: Session recording must be enabled
    on the account in order to use this API method. To enable session recording, log
    in at https://app.gotoassist.com (link is external) and go to Configure > GoToAssist
    Settings > Enable Session Recording check box.\n\n  Request Parameters                    \n
    \                     \n    field        data type      description    \n    recordingIds
    \       array      A list of RecordingIds for the recordings to be transcoded
    \   \n                      \n\nStatus Codes                \n                \n
    \   Staus Code        description    \n    204 No Content        Transcoding initiated
    \   \n    400 Bad Request        Request may be malformed or property may be missing
    or invalid    \n    403 Forbidden        Invalid authorization header or invalid
    recordingIDs    \n    500 Internal Server Error        Unexpected server error"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/archiverecordingstranscodereadyfortranscoderecordingids-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/archiverecordingstranscodereadyfortranscoderecordingids-post-openapi.md
- name: GoToAssist Remote Support - Get WebChat Transcript Info
  x-api-slug: sessionssessionidevents-get
  description: "Get information about a current or previous web-chat session based
    upon the sessionID. The session must have been run within an account or company
    that the authenticated user has access to.\n\n  Response Parameters                    \n
    \                     \n    field        data type      description    \n    sessionId
    \       string      The unique ID of this session    \n    startTime        ISO
    8601 format*      The start time of web-chat session    \n    endTime        ISO
    8601 format*      The endTime of the session    \n    timeStamp        ISO 8601
    format*      Time when the event occurred    \n    content        string      Details
    of the event. It could be a question/answer asked by customer/expert or could
    indicate joining or ending of session by expert    \n    participantName        string
    \     Name of the customer or expert    \n                      \n* ISO 8601 format
    reference\n\nStatus Codes              \n              \n    Staus Code      description
    \   \n    200 OK      WebChat transcripts info successfully fetched    \n    400
    Bad Request      An error occurred due to missing required parameters or portal
    not being created    \n    401 Unauthorized      An authentication parameter was
    passed, but either it was invalid or the technician is not entitled with a Remote
    Support seat    \n    403 Forbidden      Access denied. User doesn\u2019t have
    required roles    \n    404 Not Found      No web-chat transcript found for the
    specified session-id    \n    405 Method Not Allowed      The method was entered
    incorrectly (i.e., the technician tried to use POST, PUT etc. instead of GET)
    \   \n    500 Internal Server Error      An unhandled error occurred"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/sessionssessionidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/sessionssessionidevents-get-openapi.md
- name: GoToAssist Remote Support - Transcode Recordings
  x-api-slug: archiverecordingstranscodereadyfortranscoderecordingids-post
  description: "This method requests that a list of recordings be transcoded; once
    the API passes successfully, transcoding will be initiated for each of the recordings
    in the list. A result of \u201C204\u201D will be returned, regardless of the current
    state of the recordings (i.e., even if they are already transcoded). No more than
    500 recordings can be transcoded at once.\n\nNote: Session recording must be enabled
    on the account in order to use this API method. To enable session recording, log
    in at https://app.gotoassist.com (link is external) and go to Configure > GoToAssist
    Settings > Enable Session Recording check box.\n\n  Request Parameters                    \n
    \                     \n    field        data type      description    \n    recordingIds
    \       array      A list of RecordingIds for the recordings to be transcoded
    \   \n                      \n\nStatus Codes                \n                \n
    \   Staus Code        description    \n    204 No Content        Transcoding initiated
    \   \n    400 Bad Request        Request may be malformed or property may be missing
    or invalid    \n    403 Forbidden        Invalid authorization header or invalid
    recordingIDs    \n    500 Internal Server Error        Unexpected server error"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/archiverecordingstranscodereadyfortranscoderecordingids-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/archiverecordingstranscodereadyfortranscoderecordingids-post-openapi.md
- name: GoToAssist Remote Support - Transcode Recordings
  x-api-slug: archiverecordingstranscodereadyfortranscoderecordingids-post
  description: "This method requests that a list of recordings be transcoded; once
    the API passes successfully, transcoding will be initiated for each of the recordings
    in the list. A result of \u201C204\u201D will be returned, regardless of the current
    state of the recordings (i.e., even if they are already transcoded). No more than
    500 recordings can be transcoded at once.\n\nNote: Session recording must be enabled
    on the account in order to use this API method. To enable session recording, log
    in at https://app.gotoassist.com (link is external) and go to Configure > GoToAssist
    Settings > Enable Session Recording check box.\n\n  Request Parameters                    \n
    \                     \n    field        data type      description    \n    recordingIds
    \       array      A list of RecordingIds for the recordings to be transcoded
    \   \n                      \n\nStatus Codes                \n                \n
    \   Staus Code        description    \n    204 No Content        Transcoding initiated
    \   \n    400 Bad Request        Request may be malformed or property may be missing
    or invalid    \n    403 Forbidden        Invalid authorization header or invalid
    recordingIDs    \n    500 Internal Server Error        Unexpected server error"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/archiverecordingstranscodereadyfortranscoderecordingids-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/archiverecordingstranscodereadyfortranscoderecordingids-post-openapi.md
- name: GoToAssist Remote Support - Available Recordings
  x-api-slug: archiverecordings-get
  description: "This method retrieves a list of all available recordings on the account.
    Only recordings which are available for transcoding or downloading will be returned.
    The recording IDs are always returned in the order in which the recordings were
    started (i.e., startTime order). The request must contain one or more of the following:
    accountKey, userKey or companyId. The list of recordings can be filtered by the
    request parameters listed below.\n\nNote: Session recording must be enabled on
    the account in order to use this API method. To enable session recording, log
    in at https://app.gotoassist.com (link is external) and go to Configure > GoToAssist
    Settings > Enable Session Recording check box.\n\n  Request Parameters                  \n
    \ Each request must contain one or more of the following: accountKey, userKey
    or companyId.                  \n                    \n    field      data type
    \     description    \n    accountKey      number      The account key associated
    with the recording ( available in the Get Screen Sharing Session Info (link is
    external) method response )    \n    userKey      number      The user key of
    the technician who started the recorded session (available in the Authentication
    (link is external) API method response)    \n    companyId      number      The
    companyId associated with the recording for unattended support sessions only (
    available in the Get Companies (link is external) API method response )    \n
    \   sessionType *      number      The type of session: attended (0) or unattended
    (1)    \n    fromTime *      ISO 8601 format **      The oldest sessions that
    should be retrieved (startTime must be greater than or equal to fromTime)    \n
    \   toTime *      ISO 8601 format **      The most recent sessions that should
    be retrieved (startTime must be greater than or equal to fromTime)    \n    timePeriod
    *      number      The recordings within a Time Period, starting from currentDate
    (ex: \u201DtimePeriod=30\u201D would retrieve the last 30 days\u2019 recordings)
    \   \n    archived *      number      The option to include only archived recordings,
    as follows: include only archived recordings (1) or include only non-archived
    recordings (0 or omit)    \n                    \n* Optional                    \n**
    ISO 8601 format reference                    \n                    \n  Response
    Parameters                  \n  No more than 500 recordings at a time will be
    returned for readyForTranscode or readyForDownload.                  \n                    \n
    \   field      data type      description    \n    readyForTranscode      array
    \     A list of recordingIds for recordings that are ready to be transcoded    \n
    \   readyForDownload      array      A list of recordingIds for recordings that
    are ready to be downloaded    \n                    \n                    \nStatus
    Codes                    \n                    \n    Staus Code      description
    \         \n    200 OK      Recordings retrieved successfully          \n    400
    Bad Request      Request may be malformed or property may be missing or invalid
    \         \n    403 Forbidden      Invalid authorization header or invalid userKey,
    accountKey or companyId          \n    500 Internal Server Error      Unexpected
    server error"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/archiverecordings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/archiverecordings-get-openapi.md
- name: GoToAssist Remote Support - Get WebChat Transcript Info
  x-api-slug: sessionssessionidevents-get
  description: "Get information about a current or previous web-chat session based
    upon the sessionID. The session must have been run within an account or company
    that the authenticated user has access to.\n\n  Response Parameters                    \n
    \                     \n    field        data type      description    \n    sessionId
    \       string      The unique ID of this session    \n    startTime        ISO
    8601 format*      The start time of web-chat session    \n    endTime        ISO
    8601 format*      The endTime of the session    \n    timeStamp        ISO 8601
    format*      Time when the event occurred    \n    content        string      Details
    of the event. It could be a question/answer asked by customer/expert or could
    indicate joining or ending of session by expert    \n    participantName        string
    \     Name of the customer or expert    \n                      \n* ISO 8601 format
    reference\n\nStatus Codes              \n              \n    Staus Code      description
    \   \n    200 OK      WebChat transcripts info successfully fetched    \n    400
    Bad Request      An error occurred due to missing required parameters or portal
    not being created    \n    401 Unauthorized      An authentication parameter was
    passed, but either it was invalid or the technician is not entitled with a Remote
    Support seat    \n    403 Forbidden      Access denied. User doesn\u2019t have
    required roles    \n    404 Not Found      No web-chat transcript found for the
    specified session-id    \n    405 Method Not Allowed      The method was entered
    incorrectly (i.e., the technician tried to use POST, PUT etc. instead of GET)
    \   \n    500 Internal Server Error      An unhandled error occurred"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/sessionssessionidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transcripts/master/_listings/logmein/sessionssessionidevents-get-openapi.md
x-common:
- type: x-github
  url: https://github.com/logmein
- type: x-openapi
  url: https://www.getpostman.com/collections/94ad52bdc3d954bad52a
- type: x-postman-collection
  url: https://www.getpostman.com/collections/00bf4391e993c3afa7b7
- type: x-postman-collection
  url: https://www.getpostman.com/collections/c35d614484f21e581775
- type: x-postman-collection
  url: https://www.getpostman.com/collections/9c6e067461f45f7faa6b
- type: x-postman-collection
  url: https://drive.google.com/open?id=16WZlBkS1i8cWSfZ3mMKOwlNP-qsE7AWy
- type: x-postman-collection
  url: https://drive.google.com/file/d/1vI11FNCKpv6WJ_70hoqPNMmPAkASiOU_/view?usp=sharing
- type: x-website
  url: http://www.LogMeInInc.com
- type: x-api-gallery
  url: http://loginradius.api.gallery.streamdata.io
- type: x-api-stack
  url: http://logmein.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/logmein
- type: x-developer
  url: https://goto-developer.logmeininc.com/
- type: x-documentation
  url: https://goto-developer.logmeininc.com/apis/apis-overview
- type: x-faq
  url: https://goto-developer.logmeininc.com/faq-page
- type: x-support
  url: https://goto-developer.logmeininc.com/api-support-request-template
- type: x-twitter
  url: https://twitter.com/LogMeIn
- type: x-website
  url: https://www.logmeininc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---