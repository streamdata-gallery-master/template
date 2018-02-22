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
  /?Action=AdminGetUser&k=1:
    get:
      summary: ' Admin Get User '
      description: Gets the specified user by user name in a user pool as an administrator
      operationId: adminGetUser
      parameters:
      - in: query
        name: Username
        description: The user name of the user you wish to retrieve
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to get information
          about the            user
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