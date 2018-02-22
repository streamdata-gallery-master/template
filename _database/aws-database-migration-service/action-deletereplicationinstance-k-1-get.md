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
  /?Action=DeleteReplicationInstance&k=1:
    get:
      summary: ' Delete Replication Instance '
      description: Deletes the specified replication instance
      operationId: deleteReplicationInstance
      parameters:
      - in: query
        name: ReplicationInstanceArn
        description: The Amazon Resource Name (ARN) of the replication instance to
          be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - replication instances
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