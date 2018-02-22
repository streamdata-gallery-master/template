---
swagger: "2.0"
info:
  title: AWS Database Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartReplicationTask&k=1:
    get:
      summary: ' Start Replication Task '
      description: Starts the replication task
      operationId: startReplicationTask
      parameters:
      - in: query
        name: CdcStartTime
        description: The start time for the Change Data Capture (CDC) operation
        type: string
      - in: query
        name: ReplicationTaskArn
        description: The Amazon Resource Number (ARN) of the replication task to be
          started
        type: string
      - in: query
        name: StartReplicationTaskType
        description: The type of replication task
        type: string
      responses:
        200:
          description: OK
      tags:
      - replication tasks
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