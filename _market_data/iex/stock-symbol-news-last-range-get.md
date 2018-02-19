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
  /stock/{symbol}/news/last/{range}:
    get:
      summary: News
      description: The above example will return JSON with the following keys
      operationId: news
      parameters:
      - in: path
        name: range
        description: The date range
        type: string
        format: string
      - in: path
        name: symbol
        description: Stock ticker symbol
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - market data
      - financial news
definitions: []
x-streamrank:
  polling_total_time_average: "0.4"
  polling_size_download_average: "12122.17"
  streaming_total_time_average: "0.28"
  streaming_size_download_average: "6271.61"
  change_yes: "174"
  change_no: "1090"
  time_percentage: "29"
  size_percentage: "48"
  change_percentage: "14"
  last_run: "2018-02-15"
  days_run: "1"
  minute_run: "0"
---