---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio GetTranscriptionList
  description: GetTranscriptionList
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/Transcriptions/{TranscriptionSid}:
    delete:
      summary: Delete Transcription
      description: Deletes a transcription from your account.
      operationId: deletes-a-transcription-from-your-account
      x-api-path-slug: accountsaccountsidtranscriptionstranscriptionsid-delete
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: TranscriptionSid
        description: A 34 character string that uniquely identifies the transcription
      responses:
        200:
          description: OK
      tags:
      - Transcriptions
    get:
      summary: Get Transcription
      description: Returns a single Transcription resource representation identified
        by thengiven {TranscriptionSid}. By default Twilio will respond with the XML
        metadata for the Transcription. If you append .txt to the end of the Transcription
        resources URI Twilio will just return you the transcription tex.n
      operationId: returns-a-single-transcription-resource-representation-identified-by-thegiven-transcriptionsid-by-de
      x-api-path-slug: accountsaccountsidtranscriptionstranscriptionsid-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: TranscriptionSid
        description: A 34 character string that uniquely identifies the transcription
      responses:
        200:
          description: OK
      tags:
      - Transcriptions
  /Accounts/{AccountSid}/Transcriptions:
    get:
      summary: Get Transcriptions
      description: Returns a set of Transcription resource representations that includes
        pagingninformation.n
      operationId: returns-a-set-of-transcription-resource-representations-that-includes-paginginformation
      x-api-path-slug: accountsaccountsidtranscriptions-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Transcriptions
  /Accounts/{AccountSid}/Transcriptions.{format}:
    get:
      summary: GetTranscriptionList
      description: GetTranscriptionList
      operationId: gettranscriptionlist
      x-api-path-slug: accountsaccountsidtranscriptions-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
      responses:
        200:
          description: OK
      tags:
      - Transcriptions
  /Accounts/{AccountSid}/Transcriptions/{TranscriptionSid}.{format}:
    get:
      summary: GetTranscription
      description: GetTranscription
      operationId: gettranscription
      x-api-path-slug: accountsaccountsidtranscriptionstranscriptionsid-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
      - in: path
        name: TranscriptionSid
        description: A 34 character string that uniquely identifies the transcription
      responses:
        200:
          description: OK
      tags:
      - Transcriptions
  /Accounts/{AccountSid}/Recordings/{RecordingSid}/Transcriptions:
    get:
      summary: Get Recording Transcriptions
      description: Returns a set of Transcription resource representations that includes
        pagingninformation.n
      operationId: returns-a-set-of-transcription-resource-representations-that-includes-paginginformation
      x-api-path-slug: accountsaccountsidrecordingsrecordingsidtranscriptions-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: RecordingSid
        description: A 34 character string that uniquely identifies the recording
      responses:
        200:
          description: OK
      tags:
      - Recordings
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