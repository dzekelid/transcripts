{
  "info": {
    "name": "Twilio Delete Transcription",
    "_postman_id": "57ba4e97-4e47-4310-9d60-2a80f33467fe",
    "description": "Deletes a transcription from your account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "transcriptions",
      "item": [
        {
          "id": "6eed0c3e-cd9f-4edd-b827-2035629f249c",
          "name": "deletes-a-transcription-from-your-account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Transcriptions/:TranscriptionSid"
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "TranscriptionSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a transcription from your account"
          },
          "response": [
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "[\r\n  {\r\n    \"uri\": \"uri\",\r\n    \"firstpageuri\": \"firstpageuri\",\r\n    \"nextpageuri\": \"nextpageuri\",\r\n    \"previouspageuri\": \"previouspageuri\",\r\n    \"page\": \"page\",\r\n    \"pagesize\": \"pagesize\",\r\n    \"transcriptions\": {}\r\n  }\r\n]",
              "status": "Successful response",
              "code": 200,
              "name": "Response_200",
              "id": "b6905688-d8a1-4c0a-ac11-aa18d4e827ff"
            }
          ]
        }
      ]
    }
  ]
}