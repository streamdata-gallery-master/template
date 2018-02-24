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
  /?Action=ModifyClusterParameterGroup&k=1:
    get:
      summary: ' Modify Cluster Parameter Group '
      description: Modifies the parameters of a parameter group
      operationId: modifyClusterParameterGroup
      parameters:
      - in: query
        name: ParameterGroupName
        description: The name of the parameter group to be modified
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of parameters to be modified
        type: string
      responses:
        200:
          description: OK
      tags:
      - cluster parameter groups
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