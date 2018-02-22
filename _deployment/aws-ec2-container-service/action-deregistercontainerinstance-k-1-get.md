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
  /?Action=DeregisterContainerInstance&k=1:
    get:
      summary: ' Deregister Container Instance '
      description: Deregisters an Amazon ECS container instance from the specified
        cluster
      operationId: deregisterContainerInstance
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the container instance            to deregister
        type: string
      - in: query
        name: containerInstance
        description: The container instance ID or full Amazon Resource Name (ARN)
          of the container instance to            deregister
        type: string
      - in: query
        name: force
        description: Forces the deregistration of the container instance
        type: string
      responses:
        200:
          description: OK
      tags:
      - container instances
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