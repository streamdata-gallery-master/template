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
  /?Action=CreateSnapshot&k=1:
    get:
      summary: ' Create Snapshot '
      description: Creates a snapshot of a Simple AD or Microsoft AD directory in
        the AWS cloud
      operationId: createSnapshot
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory of which to take a snapshot
        type: string
      - in: query
        name: Name
        description: The descriptive name to apply to the snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - snapshot
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