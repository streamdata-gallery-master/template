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
  /?Action=UpdateLoginProfile&k=1:
    get:
      summary: ' Update Login Profile '
      description: Changes the password for the specified IAM user
      operationId: updateLoginProfile
      parameters:
      - in: query
        name: Password
        description: The new password for the specified IAM user
        type: string
      - in: query
        name: PasswordResetRequired
        description: Allows this new password to be used only once by requiring the
          specified IAM user to      set a new password on next sign-in
        type: string
      - in: query
        name: UserName
        description: The name of the user whose password you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - login profiles
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