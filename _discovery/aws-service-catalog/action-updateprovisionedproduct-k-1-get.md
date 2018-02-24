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
  /?Action=UpdateProvisionedProduct&k=1:
    get:
      summary: ' Update Provisioned Product '
      description: Requests updates to the configuration of an existing ProvisionedProduct
        object
      operationId: updateProvisionedProduct
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PathId
        description: The identifier of the path to use in the updated ProvisionedProduct
          object
        type: string
      - in: query
        name: ProductId
        description: The identifier of the ProvisionedProduct object
        type: string
      - in: query
        name: ProvisionedProductId
        description: The identifier of the ProvisionedProduct object to update
        type: string
      - in: query
        name: ProvisionedProductName
        description: 'The updated name of the ProvisionedProduct object '
        type: string
      - in: query
        name: ProvisioningArtifactId
        description: The provisioning artifact identifier for this product
        type: string
      - in: query
        name: ProvisioningParameters
        description: A list of ProvisioningParameter objects used to update the         ProvisionedProduct
          object
        type: string
      - in: query
        name: UpdateToken
        description: The idempotency token that uniquely identifies the provisioning
          update         request
        type: string
      responses:
        200:
          description: OK
      tags:
      - provisioned products
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