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
  /?Action=InitiateDocumentVersionUpload&k=1:
    get:
      summary: ' Initiate Document Version Upload '
      description: Creates a new document object and version object
      operationId: initiateDocumentVersionUpload
      parameters:
      - in: query
        name: ContentType
        description: The content type of the document
        type: string
      - in: query
        name: DocumentSizeInBytes
        description: The size of the document, in bytes
        type: string
      - in: query
        name: Id
        description: The ID of the document
        type: string
      - in: query
        name: Name
        description: The name of the document
        type: string
      - in: query
        name: ParentFolderId
        description: The ID of the parent folder
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