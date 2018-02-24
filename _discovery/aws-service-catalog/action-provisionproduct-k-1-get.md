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
  /?Action=ProvisionProduct&k=1:
    get:
      summary: ' Provision Product '
      description: Requests a Provision of a specified product
      operationId: provisionProduct
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: NotificationArns
        description: Passed to CloudFormation
        type: string
      - in: query
        name: PathId
        description: The identifier of the path for this product's provisioning
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      - in: query
        name: ProvisionedProductName
        description: A user-friendly name to identify the ProvisionedProduct object
        type: string
      - in: query
        name: ProvisioningArtifactId
        description: The provisioning artifact identifier for this product
        type: string
      - in: query
        name: ProvisioningParameters
        description: Parameters specified by the administrator that are required for
          provisioning the         product
        type: string
      - in: query
        name: ProvisionToken
        description: An idempotency token that uniquely identifies the provisioning
          request
        type: string
      - in: query
        name: Tags
        description: A list of tags to use as provisioning options
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