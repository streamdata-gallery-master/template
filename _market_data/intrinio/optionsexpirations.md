---
swagger: "2.0"
info:
  title: Intrinio
  description: Through our Intrinio Data Marketplace, we offer a wide selection of
    financial data feeds sourced by our own proprietary processes as well as from
    many data vendors. The primary application of the Intrinio API is for use in third-party
    applications and integrations or for end-users utilizing the Excel add-in and
    Google Sheets add-on. The Intrinio API uses HTTPS verbs and a RESTful endpoint
    structure, which makes it easy to request data from Intrinio. Basic Authentication
    is administered over HTTPS. Responses are delivered in JSON format.
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /options/expirations:
    get:
      summary: Option Expirations
      description: Returns all option contract expiration dates for a given ticker
      operationId: option-expirations
      parameters:
      - in: query
        name: ticker
        description: ' the option ticker symbol, corresponding to the underlying security'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Options
definitions: []
---