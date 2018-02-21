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
  /rawaddr/{bitcoin_address}:
    get:
      summary: Raw Address
      description: Returns a single blockchain address
      operationId: getRawAddress
      parameters:
      - in: path
        name: bitcoin_address
        description: The bitcoin address
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - blockchain
      - addresses
definitions: []
x-streamrank:
  polling_total_time_average: "4.99"
  polling_size_download_average: "4970732.31"
  streaming_total_time_average: "3.14"
  streaming_size_download_average: "2485713.99"
  change_yes: "5"
  change_no: "782"
  time_percentage: "37"
  size_percentage: "50"
  change_percentage: "1"
  last_run: "2018-02-21"
  days_run: "1"
  minute_run: "0"
---