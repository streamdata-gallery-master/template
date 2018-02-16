---
swagger: "2.0"
info:
  title: Quandl
  description: The Quandl API
  version: 1.0.0
host: www.quandl.com
basePath: /api/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /databases/{database_code}:
    get:
      summary: Get Database
      description: This call returns descriptive metadata for the specified database
      operationId: this-call-returns-descriptive-metadata-for-the-specified-database
      parameters:
      - in: path
        name: database_code
        description: The unique database code on Quandl (ex
      responses:
        200:
          description: OK
      tags:
      - Market Data
definitions: []
---