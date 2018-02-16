---
swagger: "2.0"
info:
  title: IEX Trading
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
  /stock/{symbol}/list:
    get:
      summary: List
      description: Refer to the quote section
      operationId: list
      parameters:
      - in: query
        name: displayPercent
        description: ' Optional  If set to true, all percentage values will be multiplied
          by a factor of 100 (Ex: /stock/aapl/quote?displayPercent=true)'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Quotes
definitions: []
---