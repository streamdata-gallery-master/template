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
  /datasets/{database_code}/{dataset_code}/metadata:
    get:
      summary: Get Datasets Metadata
      description: To download the metadata associated with any dataset object, append
        /metadata to your API request
      operationId: to-download-the-metadata-associated-with-any-dataset-object-append-metadata-to-your-api-request-you-
      parameters:
      - in: query
        name: column_names
      - in: path
        name: database_code
        description: The unique database code on Quandl (ex
      - in: path
        name: dataset_code
        description: The unique dataset code on Quandl (ex
      - in: query
        name: description
      - in: query
        name: frequency
      - in: query
        name: name
      - in: query
        name: newest_available_date
      - in: query
        name: oldest_available_date
      - in: query
        name: premium
      - in: query
        name: refreshed_at
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Market Data
definitions: []
---