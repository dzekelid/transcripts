{
  "info": {
    "name": "Vinli Get all transactions for this app",
    "_postman_id": "57fada98-a1ac-4760-8973-4973807590f7",
    "description": "Get all transactions for this app.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Transactionsthis",
      "item": [
        {
          "id": "0cde4cca-9f26-4c35-a419-ddea705b8723",
          "name": "TransactionsGet",
          "request": {
            "url": "http://events.vin.li/api/v1/transactions",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all transactions for this app."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c95823d5-441e-4595-b2d8-673b47ca30d3"
            }
          ]
        }
      ]
    }
  ]
}