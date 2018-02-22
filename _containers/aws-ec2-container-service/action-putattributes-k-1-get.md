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
  /?Action=PutAttributes&k=1:
    get:
      summary: ' Put Attributes '
      description: Create or update an attribute on an Amazon ECS resource
      operationId: putAttributes
      parameters:
      - in: query
        name: attributes
        description: The attributes to apply to your resource
        type: string
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that contains the resource to apply            attributes
        type: string
      responses:
        200:
          description: OK
      tags:
      - attributes
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