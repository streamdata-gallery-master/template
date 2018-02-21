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
  /unspent:
    get:
      summary: Unspent
      description: Unspent output
      operationId: getUnspentOutput
      parameters:
      - in: query
        name: active
        description: Multiple addresses divided by | Address can be base58 or xpub
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - blockchain
      - output
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