---
swagger: "2.0"
info:
  title: Intrinio API
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
  /data_point:
    get:
      summary: Data Point
      description: Returns the most recent median data point for an Economic index
        for a selected tag
      operationId: data-point
      parameters:
      - in: query
        name: identifier
        description: ' an identifier for the Economic Index selected: '
        type: string
      - in: query
        name: item
        description: ' the specified standardized tag or series ID requested: ECONOMIC
          TAGS'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Data
definitions: []
---