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
  /?Action=GetRolePolicy&k=1:
    get:
      summary: ' Get Role Policy '
      description: |-
        Retrieves the specified inline policy document that is embedded with the specified
              IAM role
      operationId: getRolePolicy
      parameters:
      - in: query
        name: PolicyName
        description: The name of the policy document to get
        type: string
      - in: query
        name: RoleName
        description: The name of the role associated with the policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - role policies
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