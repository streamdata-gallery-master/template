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
  /?Action=StartTask&k=1:
    get:
      summary: ' Start Task '
      description: |-
        Starts a new task from the specified task definition on the specified container
                    instance or instances
      operationId: startTask
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          on which to start your task
        type: string
      - in: query
        name: containerInstances
        description: The container instance IDs or full Amazon Resource Name (ARN)
          entries for the container instances on            which you would like to
          place your task
        type: string
      - in: query
        name: group
        description: The name of the task group to associate with the task
        type: string
      - in: query
        name: overrides
        description: A list of container overrides in JSON format that specify the
          name of a container            in the specified task definition and the
          overrides it should receive
        type: string
      - in: query
        name: startedBy
        description: An optional tag specified when a task is started
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to start
        type: string
      responses:
        200:
          description: OK
      tags:
      - tasks
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