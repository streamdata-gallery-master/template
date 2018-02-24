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
  /?Action=ApplyEnvironmentManagedAction&k=1:
    get:
      summary: ' Apply Environment Managed Action '
      description: Applies a scheduled managed action immediately
      operationId: applyEnvironmentManagedAction
      parameters:
      - in: query
        name: ActionId
        description: The action ID of the scheduled managed action to execute
        type: string
      - in: query
        name: EnvironmentId
        description: The environment ID of the target environment
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the target environment
        type: string
      responses:
        200:
          description: OK
      tags:
      - environments
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