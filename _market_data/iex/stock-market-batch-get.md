---
swagger: "2.0"
info:
  title: IEX
  description: The IEX API is a set of services designed for developers and engineers.
    It can be used to build high-quality apps and services. We&rsquo;re always working
    to improve the IEX API. Please check back for enhancements and improvements.
  termsOfService: https://iextrading.com/api-terms/
  version: 1.0.0
host: api.iextrading.com
basePath: /1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stock/market/batch:
    get:
      summary: Batch Requests
      description: Returns batch stock quotes
      operationId: batch-requests
      parameters:
      - in: query
        name: '*'
        description: ' Optional  Parameters that are sent to individual endpoints
          can be specified in batch calls and will be applied to each supporting endpoint'
      - in: query
        name: range
        description: ' Optional  Used to specify a chart range if chart is used in
          types parameter'
      - in: query
        name: symbols
        description: ' Optional  Comma delimited list of symbols limited to 100'
      - in: query
        name: types
        description: ' Required  Comma delimited list of endpoints to call'
      responses:
        200:
          description: OK
      tags:
      - market data
      - quotes
      - batch
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