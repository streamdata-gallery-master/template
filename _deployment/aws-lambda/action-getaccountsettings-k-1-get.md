---
swagger: "2.0"
info:
  title: AWS Lambda API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetAccountSettings&k=1:
    get:
      summary: ' Get Account Settings '
      description: Returns a customer's account settings
      operationId: getAccountSettings
      parameters:
      - in: query
        name: AccountLimit
        description: Provides limits of code size and concurrency associated with
          the current account and region
        type: string
      - in: query
        name: AccountUsage
        description: Provides code size usage and function count associated with the
          current account and region
        type: string
      responses:
        200:
          description: OK
      tags:
      - accounts
definitions: []
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