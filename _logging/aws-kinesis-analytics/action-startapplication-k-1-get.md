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
  /?Action=StartApplication&k=1:
    get:
      summary: ' Start Application '
      description: Starts the specified Amazon Kinesis Analytics application
      operationId: startApplication
      parameters:
      - in: query
        name: ApplicationName
        description: Name of the application
        type: string
      - in: query
        name: InputConfigurations
        description: Identifies the specific input, by ID, that the application starts
          consuming
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