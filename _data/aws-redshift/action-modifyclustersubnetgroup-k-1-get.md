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
  /?Action=ModifyClusterSubnetGroup&k=1:
    get:
      summary: ' Modify Cluster Subnet Group '
      description: Modifies a cluster subnet group to include the specified list of
        VPC subnets
      operationId: modifyClusterSubnetGroup
      parameters:
      - in: query
        name: ClusterSubnetGroupName
        description: The name of the subnet group to be modified
        type: string
      - in: query
        name: Description
        description: A text description of the subnet group to be modified
        type: string
      - in: query
        name: SubnetIds.SubnetIdentifier.N
        description: An array of VPC subnet IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - cluster subnet groups
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