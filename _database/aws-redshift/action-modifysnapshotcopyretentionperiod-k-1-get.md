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
  /?Action=ModifySnapshotCopyRetentionPeriod&k=1:
    get:
      summary: ' Modify Snapshot Copy Retention Period '
      description: |-
        Modifies the number of days to retain automated snapshots in the destination region
                    after they are copied from the source region
      operationId: modifySnapshotCopyRetentionPeriod
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the cluster for which you want to change
          the retention            period for automated snapshots that are copied
          to a destination region
        type: string
      - in: query
        name: RetentionPeriod
        description: The number of days to retain automated snapshots in the destination
          region after            they are copied from the source region
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