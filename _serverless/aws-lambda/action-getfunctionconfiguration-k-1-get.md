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
  /?Action=GetFunctionConfiguration&k=1:
    get:
      summary: ' Get Function Configuration '
      description: Returns the configuration information of the Lambda function
      operationId: getFunctionConfiguration
      parameters:
      - in: query
        name: FunctionName
        description: The name of the Lambda function for which you want to retrieve
          the configuration information
        type: string
      - in: query
        name: Qualifier
        description: Using this optional parameter you can specify a function version
          or an alias name
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