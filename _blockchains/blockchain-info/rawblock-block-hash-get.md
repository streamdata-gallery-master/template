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
  /rawblock/{block_hash}:
    get:
      summary: Raw Block
      description: Returns a single raw block
      operationId: getRawBlock
      parameters:
      - in: path
        name: block_hash
        description: The block hash
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - blockchain
      - blocks
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