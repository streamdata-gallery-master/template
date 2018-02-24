---
swagger: "2.0"
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RetireGrant&k=1:
    get:
      summary: ' Retire Grant '
      description: Retires a grant
      operationId: retireGrant
      parameters:
      - in: query
        name: GrantId
        description: Unique identifier of the grant to retire
        type: string
      - in: query
        name: GrantToken
        description: Token that identifies the grant to be retired
        type: string
      - in: query
        name: KeyId
        description: The Amazon Resource Name of the CMK associated with the grant
        type: string
      responses:
        200:
          description: OK
      tags:
      - grants
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