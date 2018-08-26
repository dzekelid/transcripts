{
  "info": {
    "name": "Twilio GetTranscriptionList",
    "_postman_id": "6219f8e4-c21c-42cb-b23a-45745f0c042b",
    "description": "GetTranscriptionList",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "transcriptions",
      "item": [
        {
          "id": "959ca0ce-ba8a-4380-b4a9-83e86dc883ee",
          "name": "gettranscriptionlist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twilio.com",
              "path": [
                "2010-04-01",
                "Accounts/:AccountSid/Transcriptions.json"
              ],
              "query": [
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountSid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "GetTranscriptionList"
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
              "id": "1b65dbbe-eb67-4071-a28e-702c7f1b18e8"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "The supplied credentials, if any, are not sufficient to access the resource",
              "code": 401,
              "name": "Response_401",
              "id": "e59e6700-16c6-461c-9b46-3c26d518a3dc"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "You know this one",
              "code": 404,
              "name": "Response_404",
              "id": "2492e24c-8977-452a-9816-c52944683c1f"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "Your application is sending too many simultaneous requests",
              "code": 429,
              "name": "Response_429",
              "id": "df55ebe4-de8b-4b9a-a8ca-fe16ab775d4a"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "We couldn't return the representation due to an internal server error",
              "code": 500,
              "name": "Response_500",
              "id": "004c83b3-b3a1-421b-a401-6ad8a899aa73"
            },
            {
              "header": [
                {
                  "key": "Content-Type",
                  "value": "application/json",
                  "disabled": false
                }
              ],
              "body": "{\r\n  \"Status\": \"Status\",\r\n  \"Message\": \"Message\",\r\n  \"Code\": \"Code\",\r\n  \"MoreInfo\": \"MoreInfo\"\r\n}",
              "status": "We are temporarily unable to return the representation",
              "code": 503,
              "name": "Response_503",
              "id": "c978cad5-f55f-4870-8dd7-41c7fbb9fa17"
            }
          ]
        }
      ]
    }
  ]
}