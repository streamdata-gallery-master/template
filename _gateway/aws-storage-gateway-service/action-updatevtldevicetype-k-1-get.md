---
swagger: "2.0"
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateVTLDeviceType&k=1:
    get:
      summary: ' Update VTL Device Type '
      description: Updates the type of medium changer in a gateway-VTL
      operationId: updateVTLDeviceType
      parameters:
      - in: query
        name: DeviceType
        description: The type of medium changer you want to select
        type: string
      - in: query
        name: VTLDeviceARN
        description: The Amazon Resource Name (ARN) of the medium changer you want
          to select
        type: string
      responses:
        200:
          description: OK
      tags:
      - vtl device type
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