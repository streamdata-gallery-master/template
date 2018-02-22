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
  /?Action=DescribeSnapshots&k=1:
    get:
      summary: ' Describe Snapshots '
      description: Obtains information about the directory snapshots that belong to
        this account
      operationId: describeSnapshots
      parameters:
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which to retrieve snapshot
          information
        type: string
      - in: query
        name: Limit
        description: The maximum number of objects to return
        type: string
      - in: query
        name: NextToken
        description: The DescribeSnapshotsResult
        type: string
      - in: query
        name: SnapshotIds
        description: A list of identifiers of the snapshots to obtain the information
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - snapshots
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