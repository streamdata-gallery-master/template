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
  /stats/historical:
    get:
      summary: Historical Summary
      description: See our stats page for a reference of the keys
      operationId: historical-summary
      parameters:
      - in: query
        name: date
        description: ' Parameter is optional Value needs to be in four-digit year,
          two-digit month format (YYYYMM) (i'
      - in: query
        name: format
        description: ' Parameter is optional Value can only be csv When parameter
          is not present, format defaults to JSON'
      responses:
        200:
          description: OK
      tags:
      - market data
      - historical
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