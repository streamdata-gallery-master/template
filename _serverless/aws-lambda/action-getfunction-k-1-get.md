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
  /?Action=GetFunction&k=1:
    get:
      summary: ' Get Function '
      description: "Returns the configuration information of the Lambda function and
        a presigned URL \n      link to the"
      operationId: getFunction
      parameters:
      - in: query
        name: FunctionName
        description: The Lambda function name
        type: string
      - in: query
        name: Qualifier
        description: Using this optional parameter to specify a function version or
          an alias name
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