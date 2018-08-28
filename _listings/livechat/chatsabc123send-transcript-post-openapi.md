---
swagger: "2.0"
x-collection-name: LiveChat
x-complete: 0
info:
  title: LiveChat Send chat transcript to e-mail
  description: ""
  version: 1.0.0
host: api.livechatinc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /chats/ABC123/send_transcript:
    post:
      summary: Send chat transcript to e-mail
      description: ""
      operationId: ChatsABC123SendTranscriptPost
      x-api-path-slug: chatsabc123send-transcript-post
      parameters:
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Send
      - Chat
      - Transcript
      - To
      - E-mail
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