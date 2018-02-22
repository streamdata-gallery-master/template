---
swagger: "2.0"
info:
  title: AWS Server Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartOnDemandReplicationRun&k=1:
    get:
      summary: ' Start On Demand Replication Run '
      description: The start-on-demand-replication-run API is used to start a ReplicationRun
        on demand (in addition to those that are scheduled based on your frequency)
      operationId: startOnDemandReplicationRun
      parameters:
      - in: query
        name: description
        description: 'Type: String'
        type: string
      - in: query
        name: replicationJobId
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - replication runs
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