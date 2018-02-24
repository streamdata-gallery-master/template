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
  /?Action=CreateApplication&k=1:
    get:
      summary: ' Create Application '
      description: Creates an Amazon Kinesis Analytics application
      operationId: createApplication
      parameters:
      - in: query
        name: ApplicationCode
        description: One or more SQL statements that read input data, transform it,             and
          generate output
        type: string
      - in: query
        name: ApplicationDescription
        description: Summary description of the application
        type: string
      - in: query
        name: ApplicationName
        description: Name of your Amazon Kinesis Analytics application (for example,
          sample-app)
        type: string
      - in: query
        name: Inputs
        description: Use this parameter to configure the application input
        type: string
      - in: query
        name: Outputs
        description: You can configure application output to write data from any of
          the in-application streams to up to five destinations
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