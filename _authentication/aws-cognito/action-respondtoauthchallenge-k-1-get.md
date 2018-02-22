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
  /?Action=RespondToAuthChallenge&k=1:
    get:
      summary: ' Respond To Auth Challenge '
      description: Responds to the authentication challenge
      operationId: respondToAuthChallenge
      parameters:
      - in: query
        name: ChallengeName
        description: The name of the challenge
        type: string
      - in: query
        name: ChallengeResponses
        description: The responses to the authentication challenge
        type: string
      - in: query
        name: ClientId
        description: The client ID
        type: string
      - in: query
        name: Session
        description: The session
        type: string
      responses:
        200:
          description: OK
      tags:
      - authentication challenges
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