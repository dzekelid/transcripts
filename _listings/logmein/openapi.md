swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /archive/recordings/transcode/{readyForTranscodeRecordingIds}:
    post:
      summary: Transcode Recordings
      description: "This method requests that a list of recordings be transcoded;
        once the API passes successfully, transcoding will be initiated for each of
        the recordings in the list. A result of \u201C204\u201D will be returned,
        regardless of the current state of the recordings (i.e., even if they are
        already transcoded). No more than 500 recordings can be transcoded at once.\n\nNote:
        Session recording must be enabled on the account in order to use this API
        method. To enable session recording, log in at https://app.gotoassist.com
        (link is external) and go to Configure > GoToAssist Settings > Enable Session
        Recording check box.\n\n  Request Parameters                    \n                      \n
        \   field        data type      description    \n    recordingIds        array
        \     A list of RecordingIds for the recordings to be transcoded    \n                      \n\nStatus
        Codes                \n                \n    Staus Code        description
        \   \n    204 No Content        Transcoding initiated    \n    400 Bad Request
        \       Request may be malformed or property may be missing or invalid    \n
        \   403 Forbidden        Invalid authorization header or invalid recordingIDs
        \   \n    500 Internal Server Error        Unexpected server error"
      operationId: ArchiveRecordingsTranscodeByReadyForTranscodeRecordingIdsPost
      x-api-path-slug: archiverecordingstranscodereadyfortranscoderecordingids-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: readyForTranscodeRecordingIds
      responses:
        200:
          description: OK
      tags:
      - Transcode
      - Recordings
  /sessions/{sessionId}/events:
    get:
      summary: Get WebChat Transcript Info
      description: "Get information about a current or previous web-chat session based
        upon the sessionID. The session must have been run within an account or company
        that the authenticated user has access to.\n\n  Response Parameters                    \n
        \                     \n    field        data type      description    \n
        \   sessionId        string      The unique ID of this session    \n    startTime
        \       ISO 8601 format*      The start time of web-chat session    \n    endTime
        \       ISO 8601 format*      The endTime of the session    \n    timeStamp
        \       ISO 8601 format*      Time when the event occurred    \n    content
        \       string      Details of the event. It could be a question/answer asked
        by customer/expert or could indicate joining or ending of session by expert
        \   \n    participantName        string      Name of the customer or expert
        \   \n                      \n* ISO 8601 format reference\n\nStatus Codes
        \             \n              \n    Staus Code      description    \n    200
        OK      WebChat transcripts info successfully fetched    \n    400 Bad Request
        \     An error occurred due to missing required parameters or portal not being
        created    \n    401 Unauthorized      An authentication parameter was passed,
        but either it was invalid or the technician is not entitled with a Remote
        Support seat    \n    403 Forbidden      Access denied. User doesn\u2019t
        have required roles    \n    404 Not Found      No web-chat transcript found
        for the specified session-id    \n    405 Method Not Allowed      The method
        was entered incorrectly (i.e., the technician tried to use POST, PUT etc.
        instead of GET)    \n    500 Internal Server Error      An unhandled error
        occurred"
      operationId: SessionsEventsBySessionIdGet
      x-api-path-slug: sessionssessionidevents-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: sessionId
      responses:
        200:
          description: OK
      tags:
      - WebChat
      - Transcript
      - Info
  /archive/recordings:
    get:
      summary: Available Recordings
      description: "This method retrieves a list of all available recordings on the
        account. Only recordings which are available for transcoding or downloading
        will be returned. The recording IDs are always returned in the order in which
        the recordings were started (i.e., startTime order). The request must contain
        one or more of the following: accountKey, userKey or companyId. The list of
        recordings can be filtered by the request parameters listed below.\n\nNote:
        Session recording must be enabled on the account in order to use this API
        method. To enable session recording, log in at https://app.gotoassist.com
        (link is external) and go to Configure > GoToAssist Settings > Enable Session
        Recording check box.\n\n  Request Parameters                  \n  Each request
        must contain one or more of the following: accountKey, userKey or companyId.
        \                 \n                    \n    field      data type      description
        \   \n    accountKey      number      The account key associated with the
        recording ( available in the Get Screen Sharing Session Info (link is external)
        method response )    \n    userKey      number      The user key of the technician
        who started the recorded session (available in the Authentication (link is
        external) API method response)    \n    companyId      number      The companyId
        associated with the recording for unattended support sessions only ( available
        in the Get Companies (link is external) API method response )    \n    sessionType
        *      number      The type of session: attended (0) or unattended (1)    \n
        \   fromTime *      ISO 8601 format **      The oldest sessions that should
        be retrieved (startTime must be greater than or equal to fromTime)    \n    toTime
        *      ISO 8601 format **      The most recent sessions that should be retrieved
        (startTime must be greater than or equal to fromTime)    \n    timePeriod
        *      number      The recordings within a Time Period, starting from currentDate
        (ex: \u201DtimePeriod=30\u201D would retrieve the last 30 days\u2019 recordings)
        \   \n    archived *      number      The option to include only archived
        recordings, as follows: include only archived recordings (1) or include only
        non-archived recordings (0 or omit)    \n                    \n* Optional
        \                   \n** ISO 8601 format reference                    \n                    \n
        \ Response Parameters                  \n  No more than 500 recordings at
        a time will be returned for readyForTranscode or readyForDownload.                  \n
        \                   \n    field      data type      description    \n    readyForTranscode
        \     array      A list of recordingIds for recordings that are ready to be
        transcoded    \n    readyForDownload      array      A list of recordingIds
        for recordings that are ready to be downloaded    \n                    \n
        \                   \nStatus Codes                    \n                    \n
        \   Staus Code      description          \n    200 OK      Recordings retrieved
        successfully          \n    400 Bad Request      Request may be malformed
        or property may be missing or invalid          \n    403 Forbidden      Invalid
        authorization header or invalid userKey, accountKey or companyId          \n
        \   500 Internal Server Error      Unexpected server error"
      operationId: ArchiveRecordingsGet
      x-api-path-slug: archiverecordings-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: userKey
      responses:
        200:
          description: OK
      tags:
      - Available
      - Recordings