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
  /stock/{symbol}/short-interest:
    get:
      summary: Short Interest List
      description: Refer to the Short Interest specification for further details
      operationId: iex-short-interest-list
      parameters:
      - in: query
        name: format
        description: ' Parameter is optional Value can be csv or psv When parameter
          is not present, format defaults to JSON'
      - in: path
        name: symbol
        description: Stock ticker symbol
        type: string
        format: string
      - in: query
        name: token
        description: ' Parameter is optional Value is the API token from your IEX
          user account If you have been permissioned for CUSIP information you&rsquo;ll
          receive a CUSIP field, othewise data defaults to exclude CUSIP'
      responses:
        200:
          description: OK
      tags:
      - market data
      - short interest
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