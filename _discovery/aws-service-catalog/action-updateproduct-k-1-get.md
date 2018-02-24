---
swagger: "2.0"
info:
  title: AWS Service Catalog API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateProduct&k=1:
    get:
      summary: ' Update Product '
      description: Updates an existing product
      operationId: updateProduct
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AddTags
        description: Tags to add to the existing list of tags associated with the
          product
        type: string
      - in: query
        name: Description
        description: The updated text description of the product
        type: string
      - in: query
        name: Distributor
        description: The updated distributor of the product
        type: string
      - in: query
        name: Id
        description: The identifier of the product for the update request
        type: string
      - in: query
        name: Name
        description: The updated product name
        type: string
      - in: query
        name: Owner
        description: The updated owner of the product
        type: string
      - in: query
        name: RemoveTags
        description: Tags to remove from the existing list of tags associated with
          the product
        type: string
      - in: query
        name: SupportDescription
        description: The updated support description for the product
        type: string
      - in: query
        name: SupportEmail
        description: The updated support email for the product
        type: string
      - in: query
        name: SupportUrl
        description: The updated support URL for the product
        type: string
      responses:
        200:
          description: OK
      tags:
      - products
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