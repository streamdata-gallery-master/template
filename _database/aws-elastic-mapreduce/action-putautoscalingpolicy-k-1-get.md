---
swagger: "2.0"
info:
  title: AWS Elastic MapReduce API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutAutoScalingPolicy&k=1:
    get:
      summary: ' Put Auto Scaling Policy '
      description: Creates or updates an automatic scaling policy for a core instance
        group or task instance group in an Amazon EMR cluster
      operationId: putAutoScalingPolicy
      parameters:
      - in: query
        name: AutoScalingPolicy
        description: Specifies the definition of the automatic scaling policy
        type: string
      - in: query
        name: ClusterId
        description: Specifies the ID of a cluster
        type: string
      - in: query
        name: InstanceGroupId
        description: Specifies the ID of the instance group to which the automatic
          scaling policy is applied
        type: string
      responses:
        200:
          description: OK
      tags:
      - auto scaling policies
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