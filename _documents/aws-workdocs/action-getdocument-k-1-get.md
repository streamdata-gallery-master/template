---
swagger: "2.0"
info:
  title: AWS WorkDocs API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetDocument&k=1:
    get:
      summary: ' Get Document '
      description: Retrieves the specified document object
      operationId: getDocument
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document object
        type: string
      responses:
        200:
          description: OK
      tags:
      - documents
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