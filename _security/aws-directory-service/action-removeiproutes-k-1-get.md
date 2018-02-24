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
  /?Action=RemoveIpRoutes&k=1:
    get:
      summary: ' Remove Ip Routes '
      description: Removes IP address blocks from a directory
      operationId: removeIpRoutes
      parameters:
      - in: query
        name: CidrIps
        description: IP address blocks that you want to remove
        type: string
      - in: query
        name: DirectoryId
        description: Identifier (ID) of the directory from which you want to remove
          the IP addresses
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