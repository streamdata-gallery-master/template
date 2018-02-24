---
swagger: "2.0"
info:
  title: AWS Lambda API
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
      description: Using this API you can update the function version to which the
        alias points and the alias description
      operationId: updateAlias
      parameters:
      - in: query
        name: FunctionName
        description: The function name for which the alias is created
        type: string
      - in: query
        name: Name
        description: The alias name
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