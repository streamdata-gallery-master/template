---
swagger: "2.0"
info:
  title: AWS Kinesis Analytics API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AddApplicationOutput&k=1:
    get:
      summary: ' Add Application Output '
      description: Adds an external destination to your Amazon Kinesis Analytics application
      operationId: addApplicationOutput
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the application to which you want to add the output configuration
        type: string
      - in: query
        name: CurrentApplicationVersionId
        description: Version of the application to which you want add the             output
          configuration
        type: string
      - in: query
        name: Output
        description: An array of objects, each describing one output configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - applications
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