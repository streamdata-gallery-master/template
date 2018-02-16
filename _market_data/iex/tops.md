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
  /tops:
    get:
      summary: TOPS
      description: Our eligible symbol reference is updated daily
      operationId: tops
      parameters:
      - in: query
        name: format
        description: ' Parameter is optional Value can only be csv When parameter
          is not present, format defaults to JSON'
      - in: query
        name: symbols
        description: ' Parameter is optional Value needs to be a comma-separated list
          of symbols (i'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Tops
definitions: []
---