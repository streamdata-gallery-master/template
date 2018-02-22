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
  /?Action=ListTagsForResource&k=1:
    get:
      summary: ' List Tags For Resource '
      description: Lists all cost allocation tags currently on the named resource
      operationId: listTagsForResource
      parameters:
      - in: query
        name: ResourceName
        description: The Amazon Resource Name (ARN) of the resource for which you
          want the list of tags,             for example arn:aws:elasticache:us-west-2:0123456789:cluster:myCluster             or
          arn:aws:elasticache:us-west-2:0123456789:snapshot:mySnapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - resource tags
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