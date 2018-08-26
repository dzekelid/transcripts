---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 1
info:
  title: Pay Run.IO
  description: open-scableable-transparent-payroll-api-
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Employer/{EmployerId}/RtiTransactions:
    get:
      summary: Get all RTI transactions for the employer
      description: Get links for all RTI transactions for the specified employer
      operationId: GetRtiTransactionsFromEmployer
      x-api-path-slug: employeremployeridrtitransactions-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      responses:
        200:
          description: OK
      tags:
      - RTI
      - Transactionsthe
      - Employer
---