---
swagger: "2.0"
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateMicrosoftAD&k=1:
    get:
      summary: ' Create Microsoft A D '
      description: Creates a Microsoft AD in the AWS cloud
      operationId: createMicrosoftAD
      parameters:
      - in: query
        name: Description
        description: A textual description for the directory
        type: string
      - in: query
        name: Name
        description: The fully qualified domain name for the directory, such as corp
        type: string
      - in: query
        name: Password
        description: The password for the default administrative user named Admin
        type: string
      - in: query
        name: ShortName
        description: The NetBIOS name for your domain
        type: string
      - in: query
        name: VpcSettings
        description: Contains VPC information for the CreateDirectory or CreateMicrosoftAD
          operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - microsoft ad
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