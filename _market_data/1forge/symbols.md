---
swagger: "2.0"
info:
  title: 1Forge
  description: 1Forge provides real-time quote data (bid &amp; ask) for 240+ pairs.
    To see a full list of supported currency pairs, please see the full currency pair
    list. At this time, we do not offer historical data, however, clients are more
    than welcome to archive our quotes locally for internal use.
  version: 1.0.0
host: forex.1forge.com
basePath: 1.0.3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /symbols:
    get:
      summary: Get Symbols
      description: Get a list of symbols
      operationId: getSymbols
      parameters:
      - in: query
        name: api_key
        description: The api key
        type: string
        format: string
      - in: query
        name: format
        description: The format to return
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Symbols
definitions: []
