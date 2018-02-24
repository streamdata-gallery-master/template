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
  /?Action=DeleteReplicationGroup&k=1:
    get:
      summary: ' Delete Replication Group '
      description: Deletes an existing replication group
      operationId: deleteReplicationGroup
      parameters:
      - in: query
        name: FinalSnapshotIdentifier
        description: The name of a final node group (shard) snapshot
        type: string
      - in: query
        name: ReplicationGroupId
        description: The identifier for the cluster to be deleted
        type: string
      - in: query
        name: RetainPrimaryCluster
        description: If set to true, all of the read replicas are deleted,             but
          the primary node is retained
        type: string
      responses:
        200:
          description: OK
      tags:
      - replication groups
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