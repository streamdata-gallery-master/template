---
swagger: "2.0"
info:
  title: Quandl API
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
  /databases/{database_code}/data:
    get:
      summary: Get Data
      description: You can download all the data in a premium database in a single
        call, by appending /data to your database request
      operationId: you-can-download-all-the-data-in-a-premium-database-in-a-single-call-by-appending-data-to-your-datab
      parameters:
      - in: path
        name: database_code
        description: The unique database code on Quandl (ex
      - in: query
        name: download_type
        description: Data returned can be either partial or complete
      responses:
        200:
          description: OK
      tags:
      - Market Data
definitions: []
---