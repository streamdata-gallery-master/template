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
  /?Action=DescribeSnapshots&k=1:
    get:
      summary: ' Describe Snapshots '
      description: Returns information about cache cluster or replication group snapshots
      operationId: describeSnapshots
      parameters:
      - in: query
        name: CacheClusterId
        description: A user-supplied cluster identifier
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      - in: query
        name: ReplicationGroupId
        description: A user-supplied replication group identifier
        type: string
      - in: query
        name: ShowNodeGroupConfig
        description: A Boolean value which if true, the node group (shard) configuration
          is included in the snapshot description
        type: string
      - in: query
        name: SnapshotName
        description: A user-supplied name of the snapshot
        type: string
      - in: query
        name: SnapshotSource
        description: If set to system, the output shows snapshots that were automatically
          created by ElastiCache
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