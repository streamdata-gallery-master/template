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
  /?Action=CreateApplication&k=1:
    get:
      summary: ' Create Application '
      description: |-
        Creates an application that has one configuration template named default
              and no application versions
      operationId: createApplication
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application
        type: string
      - in: query
        name: Description
        description: Describes the application
        type: string
      - in: query
        name: ResourceLifecycleConfig
        description: Specify an application resource lifecycle configuration to prevent
          your application      from accumulating too many versions
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