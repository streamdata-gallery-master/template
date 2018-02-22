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
  /?Action=ListUsers&k=1:
    get:
      summary: ' List Users '
      description: Lists the users in the Amazon Cognito user pool
      operationId: listUsers
      parameters:
      - in: query
        name: AttributesToGet
        description: The attributes to get from the request to list users
        type: string
      - in: query
        name: Filter
        description: The filter for the list users request
        type: string
      - in: query
        name: Limit
        description: The limit of the request to list users
        type: string
      - in: query
        name: PaginationToken
        description: An identifier that was returned from the previous call to this
          operation, which can            be used to return the next set of items
          in the list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for which you want to list users
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