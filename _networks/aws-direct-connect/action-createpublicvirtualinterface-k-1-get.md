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
  /?Action=CreatePublicVirtualInterface&k=1:
    get:
      summary: ' Create Public Virtual Interface '
      description: Creates a new public virtual interface
      operationId: createPublicVirtualInterface
      parameters:
      - in: query
        name: connectionId
        description: ID of the connection
        type: string
      - in: query
        name: newPublicVirtualInterface
        description: Detailed information for the public virtual interface to be created
        type: string
      responses:
        200:
          description: OK
      tags:
      - private virtual interfaces
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