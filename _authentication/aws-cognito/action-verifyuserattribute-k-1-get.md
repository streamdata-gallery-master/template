---
swagger: "2.0"
info:
  title: AWs Cognito Identity Provider API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=VerifyUserAttribute&k=1:
    get:
      summary: ' Verify User Attribute '
      description: Verifies the specified user attributes in the user pool
      operationId: verifyUserAttribute
      parameters:
      - in: query
        name: AccessToken
        description: Represents the access token of the request to verify user attributes
        type: string
      - in: query
        name: AttributeName
        description: The attribute name in the request to verify user attributes
        type: string
      - in: query
        name: Code
        description: The verification code in the request to verify user attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - users
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