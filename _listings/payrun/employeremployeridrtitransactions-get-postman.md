{
  "info": {
    "name": "Pay Run.IO Get all RTI transactions for the employer",
    "_postman_id": "1625dca8-6997-455c-b1a0-dadd8886f988",
    "description": "Get links for all RTI transactions for the specified employer",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "RTI",
      "item": [
        {
          "id": "287319d1-ec0d-4ef3-80e9-fe05c71d6862",
          "name": "GetRtiTransactionsFromEmployer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/RtiTransactions"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get links for all RTI transactions for the specified employer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98c44aeb-ae52-416a-a29c-64d45d9e2be0"
            }
          ]
        }
      ]
    }
  ]
}