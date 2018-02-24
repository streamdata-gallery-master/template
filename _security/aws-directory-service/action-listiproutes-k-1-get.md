---
swagger: "2.0"
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListIpRoutes&k=1:
    get:
      summary: ' List Ip Routes '
      description: Lists the address blocks that you have added to a directory
      operationId: listIpRoutes
      parameters:
      - in: query
        name: DirectoryId
        description: Identifier (ID) of the directory for which you want to retrieve
          the IP addresses
        type: string
      - in: query
        name: Limit
        description: Maximum number of items to return
        type: string
      - in: query
        name: NextToken
        description: The ListIpRoutes
        type: string
      responses:
        200:
          description: OK
      tags:
      - ip address routes
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