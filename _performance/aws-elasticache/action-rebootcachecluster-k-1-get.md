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
  /?Action=RebootCacheCluster&k=1:
    get:
      summary: ' Reboot Cache Cluster '
      description: |-
        Reboots some, or all, of the cache nodes
                    within a provisioned cache cluster
      operationId: rebootCacheCluster
      parameters:
      - in: query
        name: CacheClusterId
        description: The cache cluster identifier
        type: string
      - in: query
        name: CacheNodeIdsToReboot.CacheNodeId.N
        description: A list of cache node IDs to reboot
        type: string
      responses:
        200:
          description: OK
      tags:
      - cache clusters
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