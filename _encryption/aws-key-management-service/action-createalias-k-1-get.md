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
  /?Action=CreateAlias&k=1:
    get:
      summary: ' Create Alias '
      description: Creates a display name for a customer master key
      operationId: createAlias
      parameters:
      - in: query
        name: AliasName
        description: String that contains the display name
        type: string
      - in: query
        name: TargetKeyId
        description: An identifier of the key for which you are creating the alias
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