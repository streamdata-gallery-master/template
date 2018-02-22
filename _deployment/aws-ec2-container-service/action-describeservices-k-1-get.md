---
swagger: "2.0"
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeServices&k=1:
    get:
      summary: ' Describe Services '
      description: Describes the specified services running in your cluster
      operationId: describeServices
      parameters:
      - in: query
        name: cluster
        description: The name of the cluster that hosts the service to describe
        type: string
      - in: query
        name: services
        description: A list of services to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - services
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