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
  /?Action=TerminateProvisionedProduct&k=1:
    get:
      summary: ' Terminate Provisioned Product '
      description: Requests termination of an existing ProvisionedProduct object
      operationId: terminateProvisionedProduct
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: IgnoreErrors
        description: If set to true, AWS Service Catalog stops managing the specified
          ProvisionedProduct object even         if it cannot delete the underlying
          resources
        type: string
      - in: query
        name: ProvisionedProductId
        description: The identifier of the ProvisionedProduct object to terminate
        type: string
      - in: query
        name: ProvisionedProductName
        description: The name of the ProvisionedProduct object to terminate
        type: string
      - in: query
        name: TerminateToken
        description: An idempotency token that uniquely identifies the termination
          request
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