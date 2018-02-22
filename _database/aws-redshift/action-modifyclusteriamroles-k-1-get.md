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
  /?Action=ModifyClusterIamRoles&k=1:
    get:
      summary: ' Modify Cluster Iam Roles '
      description: |-
        Modifies the list of AWS Identity and Access Management (IAM) roles that can be
                    used by the cluster to access other AWS services
      operationId: modifyClusterIamRoles
      parameters:
      - in: query
        name: AddIamRoles.IamRoleArn.N
        description: Zero or more IAM roles to associate with the cluster
        type: string
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the cluster for which you want to associate
          or            disassociate IAM roles
        type: string
      - in: query
        name: RemoveIamRoles.IamRoleArn.N
        description: Zero or more IAM roles in ARN format to disassociate from the
          cluster
        type: string
      responses:
        200:
          description: OK
      tags:
      - cluster iam roles
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