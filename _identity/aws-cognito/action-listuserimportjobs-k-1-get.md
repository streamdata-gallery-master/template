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
  /?Action=ListUserImportJobs&k=1:
    get:
      summary: ' List User Import Jobs '
      description: Lists the user import jobs
      operationId: listUserImportJobs
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of import jobs you want the request to return
        type: string
      - in: query
        name: PaginationToken
        description: An identifier that was returned from the previous call to ListUserImportJobs,
          which            can be used to return the next set of import jobs in the
          list
        type: string
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are being imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - user imports
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