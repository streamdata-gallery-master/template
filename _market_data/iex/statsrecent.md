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
  /stats/recent:
    get:
      summary: Recent
      description: This call will return a minimum of the last five trading days up
        to all trading days of the current month
      operationId: recent
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Statistics
definitions: []
---