---
swagger: "2.0"
info:
  title: Blockchain Info
  description: Use Blockchain's APIs at no cost to help you start building bitcoin
    apps.
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blocks/{pool_name}:
    get:
      summary: Blocks by Pool
      description: Returns the blocks for one pool
      operationId: getPoolBlocks
      parameters:
      - in: query
        name: format
        description: The format to return (json,html)
        type: string
        format: string
      - in: path
        name: pool_name
        description: The pool name
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - blockchain
      - pools
definitions: []
x-streamrank:
  polling_total_time_average: ~
  polling_size_download_average: ~
  streaming_total_time_average: ~
  streaming_size_download_average: ~
  change_yes: ~
  change_no: ~
  time_percentage: ~
  size_percentage: ~
  change_percentage: ~
  last_run: ~
  days_run: ~
  minute_run: ~
---