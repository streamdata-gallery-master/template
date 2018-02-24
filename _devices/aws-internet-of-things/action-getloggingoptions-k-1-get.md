---
swagger: "2.0"
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetLoggingOptions&k=1:
    get:
      summary: ' Get Logging Options '
      description: Gets the logging options
      operationId: getLoggingOptions
      parameters:
      - in: query
        name: logLevel
        description: The logging level
        type: string
      - in: query
        name: roleArn
        description: The ARN of the IAM role that grants access
        type: string
      responses:
        200:
          description: OK
      tags:
      - logging options
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