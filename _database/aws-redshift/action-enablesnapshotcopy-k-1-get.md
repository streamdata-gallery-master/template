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
  /?Action=EnableSnapshotCopy&k=1:
    get:
      summary: ' Enable Snapshot Copy '
      description: |-
        Enables the automatic copy of snapshots from one region to another region for a
                    specified cluster
      operationId: enableSnapshotCopy
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the source cluster to copy snapshots
          from
        type: string
      - in: query
        name: DestinationRegion
        description: The destination region that you want to copy snapshots to
        type: string
      - in: query
        name: RetentionPeriod
        description: The number of days to retain automated snapshots in the destination
          region after            they are copied from the source region
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant to use when snapshots of
          an AWS KMS-encrypted            cluster are copied to the destination region
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