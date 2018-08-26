---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToAssist Remote Support Transcode Recordings
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
  version: 1.0.0
host: api.getgo.com
basePath: /G2A/rest/v1
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---