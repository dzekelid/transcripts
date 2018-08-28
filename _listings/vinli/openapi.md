swagger: "2.0"
x-collection-name: Vinli
x-complete: 1
info:
  title: Vinli
  description: todo-add-description
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /transactions:
    get:
      summary: Get all transactions for this app
      description: Get all transactions for this app.
      operationId: TransactionsGet
      x-api-path-slug: transactions-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Transactionsthis
      - App