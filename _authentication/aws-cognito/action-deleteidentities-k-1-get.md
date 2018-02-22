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
  /?Action=DeleteIdentities&k=1:
    get:
      summary: ' Delete Identities '
      description: Deletes identities from an identity pool
      operationId: deleteIdentities
      parameters:
      - in: query
        name: IdentityIdsToDelete
        description: A list of 1-60 identities that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - identities
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