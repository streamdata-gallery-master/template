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
  /?Action=DeleteApplicationVersion&k=1:
    get:
      summary: ' Delete Application Version '
      description: Deletes the specified version from the specified application
      operationId: deleteApplicationVersion
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application to which the version belongs
        type: string
      - in: query
        name: DeleteSourceBundle
        description: Set to true to delete the source bundle from your storage bucket
        type: string
      - in: query
        name: VersionLabel
        description: The label of the version to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - application version
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