---
swagger: "2.0"
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateApplicationVersion&k=1:
    get:
      summary: ' Update Application Version '
      description: Updates the specified application version to have the specified
        properties
      operationId: updateApplicationVersion
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application associated with this version
        type: string
      - in: query
        name: Description
        description: A new description for this version
        type: string
      - in: query
        name: VersionLabel
        description: The name of the version to update
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