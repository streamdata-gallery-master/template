---
swagger: "2.0"
info:
  title: AWS ElastiCache API
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
      description: |-
        Creates a copy of an entire cache cluster or replication group at a
                    specific moment in time
      operationId: createSnapshot
      parameters:
      - in: query
        name: CacheClusterId
        description: The identifier of an existing cache cluster
        type: string
      - in: query
        name: ReplicationGroupId
        description: The identifier of an existing replication group
        type: string
      - in: query
        name: SnapshotName
        description: A name for the snapshot being created
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