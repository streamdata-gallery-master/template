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
  /hist:
    get:
      summary: HIST
      description: HIST will provide the output of IEX data products for download
        on a T+1 basis
      operationId: hist
      parameters:
      - in: query
        name: date
        description: ' Parameter is optional Value needs to be in four-digit year,
          two-digit month, two-digit day format (YYYYMMDD) (i'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
definitions: []
---