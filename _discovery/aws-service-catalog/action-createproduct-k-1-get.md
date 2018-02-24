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
  /?Action=CreateProduct&k=1:
    get:
      summary: ' Create Product '
      description: Creates a new product
      operationId: createProduct
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Description
        description: The text description of the product
        type: string
      - in: query
        name: Distributor
        description: The distributor of the product
        type: string
      - in: query
        name: IdempotencyToken
        description: A token to disambiguate duplicate requests
        type: string
      - in: query
        name: Name
        description: The name of the product
        type: string
      - in: query
        name: Owner
        description: The owner of the product
        type: string
      - in: query
        name: ProductType
        description: The type of the product to create
        type: string
      - in: query
        name: ProvisioningArtifactParameters
        description: Parameters for the provisioning artifact
        type: string
      - in: query
        name: SupportDescription
        description: Support information about the product
        type: string
      - in: query
        name: SupportEmail
        description: Contact email for product support
        type: string
      - in: query
        name: SupportUrl
        description: Contact URL for product support
        type: string
      - in: query
        name: Tags
        description: Tags to associate with the new product
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