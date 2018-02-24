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
  /?Action=DescribeDocumentVersions&k=1:
    get:
      summary: ' Describe Document Versions '
      description: Retrieves the document versions for the specified document
      operationId: describeDocumentVersions
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      - in: query
        name: Fields
        description: Specify SOURCE to include initialized versions and a URL for
          the source document
        type: string
      - in: query
        name: Include
        description: A comma-separated list of values
        type: string
      - in: query
        name: Limit
        description: The maximum number of versions to return with this call
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
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