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
  /?Action=GetRole&k=1:
    get:
      summary: ' Get Role '
      description: |-
        Retrieves information about the specified role, including the role's path, GUID, ARN,
              and the role's trust policy that grants permission to assume the role
      operationId: getRole
      parameters:
      - in: query
        name: RoleName
        description: The name of the IAM role to get information about
        type: string
      responses:
        200:
          description: OK
      tags:
      - roles
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