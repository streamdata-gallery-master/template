---
swagger: "2.0"
info:
  title: AWS CloudSearch Document Service API
  description: You use the document service API to add, replace, or delete documents
    in your Amazon CloudSearch domain. For more information managing the documents
    in your search domain, see Uploading Data to an Amazon CloudSearch Domain.
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-01-01/documents/batch:
    get:
      summary: Search Documents
      description: You use the document service API to add, replace, or delete documents
        in your Amazon CloudSearch domain
      operationId: search
      parameters:
      - in: body
        name: fields
        description: A collection of one or more field_name properties that define
          the fields the document contains
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: field_name
        description: "\tSpecifies a field within the document being added"
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: id
        description: An alphanumeric string
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: type
        description: The operation type, add or delete
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - search
definitions: []
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---