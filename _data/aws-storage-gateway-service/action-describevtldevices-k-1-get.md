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
  /?Action=DescribeVTLDevices&k=1:
    get:
      summary: ' Describe VTL Devices '
      description: |-
        Returns a description of virtual tape library (VTL) devices for the specified
                 gateway
      operationId: describeVTLDevices
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      - in: query
        name: Limit
        description: Specifies that the number of VTL devices described be limited
          to the specified         number
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          describing the VTL         devices
        type: string
      - in: query
        name: VTLDeviceARNs
        description: An array of strings, where each string represents the Amazon
          Resource Name (ARN) of a         VTL device
        type: string
      responses:
        200:
          description: OK
      tags:
      - vtl devices
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