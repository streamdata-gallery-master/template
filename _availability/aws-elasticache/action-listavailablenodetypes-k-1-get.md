---
swagger: "2.0"
info:
  title: AWS ElastiCache API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListAvailableNodeTypes&k=1:
    get:
      summary: ' List Available Node Types '
      description: ""
      operationId: listAvailableNodeTypes
      parameters:
      - in: query
        name: AvailableNodeTypes.member.N
        description: 'Type: array of AvailableNodeType objects'
        type: string
      responses:
        200:
          description: OK
      tags:
      - node types
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