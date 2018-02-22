---
swagger: "2.0"
info:
  title: AWS Directory Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=StartSchemaExtension&k=1:
    get:
      summary: ' Start Schema Extension '
      description: Applies a schema extension to a Microsoft AD directory
      operationId: startSchemaExtension
      parameters:
      - in: query
        name: CreateSnapshotBeforeSchemaExtension
        description: If true, creates a snapshot of the directory before applying
          the schema extension
        type: string
      - in: query
        name: Description
        description: A description of the schema extension
        type: string
      - in: query
        name: DirectoryId
        description: The identifier of the directory for which the schema extension
          will be applied to
        type: string
      - in: query
        name: LdifContent
        description: The LDIF file represented as a string
        type: string
      responses:
        200:
          description: OK
      tags:
      - schema extension
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