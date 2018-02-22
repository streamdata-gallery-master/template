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
  /?Action=UpdateAssumeRolePolicy&k=1:
    get:
      summary: ' Update Assume Role Policy '
      description: Updates the policy that grants an IAM entity permission to assume
        a role
      operationId: updateAssumeRolePolicy
      parameters:
      - in: query
        name: PolicyDocument
        description: The policy that grants an entity permission to assume the role
        type: string
      - in: query
        name: RoleName
        description: The name of the role to update with the new policy
        type: string
      responses:
        200:
          description: OK
      tags:
      - assume role policy
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