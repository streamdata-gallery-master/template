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
  /?Action=UpdateUserPoolClient&k=1:
    get:
      summary: ' Update User Pool Client '
      description: |-
        Allows the developer to update the specified user pool client and password
                    policy
      operationId: updateUserPoolClient
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: ClientName
        description: The client name from the update user pool client request
        type: string
      - in: query
        name: ExplicitAuthFlows
        description: Explicit authentication flows
        type: string
      - in: query
        name: ReadAttributes
        description: The read-only attributes of the user pool
        type: string
      - in: query
        name: RefreshTokenValidity
        description: The validity of the refresh token, in days
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool where you want to update the
          user pool            client
        type: string
      - in: query
        name: WriteAttributes
        description: The writeable attributes of the user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - user pool clients
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