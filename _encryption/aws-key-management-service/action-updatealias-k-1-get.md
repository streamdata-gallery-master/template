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
  /?Action=UpdateAlias&k=1:
    get:
      summary: ' Update Alias '
      description: Updates an alias to map it to a different key
      operationId: updateAlias
      parameters:
      - in: query
        name: AliasName
        description: String that contains the name of the alias to be modified
        type: string
      - in: query
        name: TargetKeyId
        description: Unique identifier of the customer master key to be mapped to
          the alias
        type: string
      responses:
        200:
          description: OK
      tags:
      - aliases
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