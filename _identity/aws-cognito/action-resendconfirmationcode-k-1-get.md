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
  /?Action=ResendConfirmationCode&k=1:
    get:
      summary: ' Resend Confirmation Code '
      description: |-
        Resends the confirmation (for confirmation of registration) to a specific user in
                    the user pool
      operationId: resendConfirmationCode
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: SecretHash
        description: A keyed-hash message authentication code (HMAC) calculated using
          the secret key of            a user pool client and username plus the client
          ID in the message
        type: string
      - in: query
        name: Username
        description: The user name of the user to whom you wish to resend a confirmation
          code
        type: string
      responses:
        200:
          description: OK
      tags:
      - confirmation code
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