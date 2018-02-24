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
  /?Action=RevokeClusterSecurityGroupIngress&k=1:
    get:
      summary: ' Revoke Cluster Security Group Ingress '
      description: |-
        Revokes an ingress rule in an Amazon Redshift security group for a previously authorized
                    IP range or Amazon EC2 security group
      operationId: revokeClusterSecurityGroupIngress
      parameters:
      - in: query
        name: CIDRIP
        description: The IP range for which to revoke access
        type: string
      - in: query
        name: ClusterSecurityGroupName
        description: The name of the security Group from which to revoke the ingress
          rule
        type: string
      - in: query
        name: EC2SecurityGroupName
        description: The name of the EC2 Security Group whose access is to be revoked
        type: string
      - in: query
        name: EC2SecurityGroupOwnerId
        description: The AWS account number of the owner of the security group specified
          in the                EC2SecurityGroupName parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - cluster security group
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