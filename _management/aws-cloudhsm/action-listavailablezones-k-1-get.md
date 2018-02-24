---
swagger: "2.0"
info:
  title: AWS CloudHSM API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListAvailableZones&k=1:
    get:
      summary: ' List Available Zones '
      description: Lists the Availability Zones that have available AWS CloudHSM capacity
      operationId: listAvailableZones
      parameters:
      - in: query
        name: AZList
        description: The list of Availability Zones that have available AWS CloudHSM
          capacity
        type: string
      responses:
        200:
          description: OK
      tags:
      - zones
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