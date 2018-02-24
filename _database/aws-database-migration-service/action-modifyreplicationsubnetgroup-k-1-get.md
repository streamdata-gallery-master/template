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
  /?Action=ModifyReplicationSubnetGroup&k=1:
    get:
      summary: ' Modify Replication Subnet Group '
      description: Modifies the settings for the specified replication subnet group
      operationId: modifyReplicationSubnetGroup
      parameters:
      - in: query
        name: ReplicationSubnetGroupDescription
        description: The description of the replication instance subnet group
        type: string
      - in: query
        name: ReplicationSubnetGroupIdentifier
        description: The name of the replication instance subnet group
        type: string
      - in: query
        name: SubnetIds
        description: A list of subnet IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - replication subnet groups
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