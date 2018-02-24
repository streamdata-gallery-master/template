---
swagger: "2.0"
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeactivateMFADevice&k=1:
    get:
      summary: ' Deactivate M F A Device '
      description: |-
        Deactivates the specified MFA device and removes it from association with the user name
              for which it was originally enabled
      operationId: deactivateMFADevice
      parameters:
      - in: query
        name: SerialNumber
        description: The serial number that uniquely identifies the MFA device
        type: string
      - in: query
        name: UserName
        description: The name of the user whose MFA device you want to deactivate
        type: string
      responses:
        200:
          description: OK
      tags:
      - virtual mfa device
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