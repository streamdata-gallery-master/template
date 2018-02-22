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
  /?Action=AdminRespondToAuthChallenge&k=1:
    get:
      summary: ' Admin Respond To Auth Challenge '
      description: Responds to an authentication challenge, as an administrator
      operationId: adminRespondToAuthChallenge
      parameters:
      - in: query
        name: ChallengeName
        description: The name of the challenge
        type: string
      - in: query
        name: ChallengeResponses
        description: The challenge response
        type: string
      - in: query
        name: ClientId
        description: The client ID
        type: string
      - in: query
        name: Session
        description: The session
        type: string
      - in: query
        name: UserPoolId
        description: The ID of the Amazon Cognito user pool
        type: string
      responses:
        200:
          description: OK
      tags:
      - authentication challenge
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