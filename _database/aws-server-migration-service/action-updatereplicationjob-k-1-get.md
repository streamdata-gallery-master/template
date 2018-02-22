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
  /?Action=UpdateReplicationJob&k=1:
    get:
      summary: ' Update Replication Job '
      description: The update-replication-job API is used to change the settings of
        your existing ReplicationJob created using CreateReplicationJob
      operationId: updateReplicationJob
      parameters:
      - in: query
        name: description
        description: 'Type: String'
        type: string
      - in: query
        name: frequency
        description: 'Type: Integer'
        type: string
      - in: query
        name: licenseType
        description: 'Type: String'
        type: string
      - in: query
        name: nextReplicationRunStartTime
        description: 'Type: Timestamp'
        type: string
      - in: query
        name: replicationJobId
        description: 'Type: String'
        type: string
      - in: query
        name: roleName
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - replication jobs
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