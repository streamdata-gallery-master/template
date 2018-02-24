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
  /?Action=RevokeCacheSecurityGroupIngress&k=1:
    get:
      summary: ' Revoke Cache Security Group Ingress '
      description: |-
        Revokes ingress from a cache
                    security group
      operationId: revokeCacheSecurityGroupIngress
      parameters:
      - in: query
        name: CacheSecurityGroupName
        description: The name of the cache security group to revoke ingress from
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The name of the Amazon EC2 security group to revoke access from
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the Amazon EC2 security group owner
        type: string
      responses:
        200:
          description: OK
      tags:
      - cache security groups
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