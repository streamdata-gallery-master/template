---
swagger: "2.0"
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DisableSnapshotCopy&k=1:
    get:
      summary: ' Disable Snapshot Copy '
      description: |-
        Disables the automatic copying of snapshots from one region to another region for a
                    specified cluster
      operationId: disableSnapshotCopy
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the source cluster that you want to
          disable copying of            snapshots to a destination region
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