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
  /?Action=DeleteApplicationReferenceDataSource&k=1:
    get:
      summary: ' Delete Application Reference Data Source '
      description: Deletes a reference data source configuration from the specified
        application configuration
      operationId: deleteApplicationReferenceDataSource
      parameters:
      - in: query
        name: ApplicationName
        description: Name of an existing application
        type: string
      - in: query
        name: CurrentApplicationVersionId
        description: Version of the application
        type: string
      - in: query
        name: ReferenceId
        description: ID of the reference data source
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