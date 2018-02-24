---
swagger: "2.0"
info:
  title: AWS Direct Connect API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateBGPPeer&k=1:
    get:
      summary: ' Create B G P Peer '
      description: Creates a new BGP peer on a specified virtual interface
      operationId: createBGPPeer
      parameters:
      - in: query
        name: newBGPPeer
        description: Detailed information for the BGP peer to be created
        type: string
      - in: query
        name: virtualInterfaceId
        description: The ID of the virtual interface on which the BGP peer will be
          provisioned
        type: string
      responses:
        200:
          description: OK
      tags:
      - bgp peer
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