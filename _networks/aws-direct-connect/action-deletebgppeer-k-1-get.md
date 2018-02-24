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
  /?Action=DeleteBGPPeer&k=1:
    get:
      summary: ' Delete B G P Peer '
      description: Deletes a BGP peer on the specified virtual interface that matches
        the specified customer address and ASN
      operationId: deleteBGPPeer
      parameters:
      - in: query
        name: asn
        description: Autonomous system (AS) number for Border Gateway Protocol (BGP)
          configuration
        type: string
      - in: query
        name: customerAddress
        description: IP address assigned to the customer interface
        type: string
      - in: query
        name: virtualInterfaceId
        description: The ID of the virtual interface from which the BGP peer will
          be deleted
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