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
  /?Action=DeleteFunction&k=1:
    get:
      summary: ' Delete Function '
      description: Deletes the specified Lambda function code and configuration
      operationId: deleteFunction
      parameters:
      - in: query
        name: FunctionName
        description: The Lambda function to delete
        type: string
      - in: query
        name: Qualifier
        description: Using this optional parameter you can specify a function version       (but
          not the $LATEST version) to direct AWS Lambda to delete a       specific
          function version
        type: string
      responses:
        200:
          description: OK
      tags:
      - functions
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