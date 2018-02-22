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
  /?Action=AddApplicationInput&k=1:
    get:
      summary: ' Add Application Input '
      description: Adds a streaming source to your Amazon Kinesis application
      operationId: addApplicationInput
      parameters:
      - in: query
        name: ApplicationName
        description: Name of your existing Amazon Kinesis Analytics application to
          which you want to add the streaming source
        type: string
      - in: query
        name: CurrentApplicationVersionId
        description: Current version of your Amazon Kinesis Analytics application
        type: string
      - in: query
        name: Input
        description: When you configure the application input, you specify the streaming
          source,  the         in-application stream name that is created, and the
          mapping between the two
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