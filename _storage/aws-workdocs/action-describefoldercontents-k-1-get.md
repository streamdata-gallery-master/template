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
  /?Action=DescribeFolderContents&k=1:
    get:
      summary: ' Describe Folder Contents '
      description: Describes the contents of the specified folder, including its documents
        and sub-folders
      operationId: describeFolderContents
      parameters:
      - in: query
        name: FolderId
        description: The ID of the folder
        type: string
      - in: query
        name: Include
        description: The contents to include
        type: string
      - in: query
        name: Limit
        description: The maximum number of items to return with this call
        type: string
      - in: query
        name: Marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: Order
        description: The order for the contents of the folder
        type: string
      - in: query
        name: Sort
        description: The sorting criteria
        type: string
      - in: query
        name: Type
        description: The type of items
        type: string
      responses:
        200:
          description: OK
      tags:
      - folders
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