---
swagger: "2.0"
info:
  title: AWS Cognito API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetIdentityPoolRoles&k=1:
    get:
      summary: ' Set Identity Pool Roles '
      description: Sets the roles for an identity pool
      operationId: setIdentityPoolRoles
      parameters:
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: RoleMappings
        description: How users for a specific identity provider are to mapped to roles
        type: string
      - in: query
        name: Roles
        description: The map of roles associated with this pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - identity pool
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