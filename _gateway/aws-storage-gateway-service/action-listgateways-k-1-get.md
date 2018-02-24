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
  /?Action=ListGateways&k=1:
    get:
      summary: ' List Gateways '
      description: Lists gateways owned by an AWS account in a region specified in
        the request
      operationId: listGateways
      parameters:
      - in: query
        name: Limit
        description: Specifies that the list of gateways returned be limited to the
          specified number of         items
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          the returned list of         gateways
        type: string
      responses:
        200:
          description: OK
      tags:
      - gateways
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