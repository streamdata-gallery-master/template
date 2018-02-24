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
  /?Action=ListAllowedNodeTypeModifications&k=1:
    get:
      summary: ' List Allowed Node Type Modifications '
      description: |-
        Lists all available node types that you
                    can scale your Redis cluster's or replication group's current node type up to
      operationId: listAllowedNodeTypeModifications
      parameters:
      - in: query
        name: CacheClusterId
        description: The name of the cache cluster you want to scale up to a larger
          node instanced type
        type: string
      - in: query
        name: ReplicationGroupId
        description: The name of the replication group want to scale up to a larger
          node type
        type: string
      responses:
        200:
          description: OK
      tags:
      - node type modifications
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