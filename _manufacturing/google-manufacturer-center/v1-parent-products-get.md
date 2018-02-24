---
swagger: "2.0"
info:
  title: Manufacturer Center
  description: Public API for managing Manufacturer Center related data.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: manufacturers.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{parent}/products:
    get:
      summary: Get Products
      description: Lists all the products in a Manufacturer Center account
      operationId: manufacturers.accounts.products.list
      parameters:
      - in: query
        name: pageSize
        description: |-
          Maximum number of product statuses to return in the response, used for
          paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      - in: path
        name: parent
        description: Parent ID in the format `accounts/{account_id}`
      responses:
        200:
          description: OK
      tags:
      - product
definitions:
  Attributes:
    properties:
      brand:
        description: This is a default description.
        type: parameters
      gtin:
        description: This is a default description.
        type: parameters
      mpn:
        description: This is a default description.
        type: parameters
      productLine:
        description: This is a default description.
        type: parameters
      productName:
        description: This is a default description.
        type: parameters
      productPageUrl:
        description: This is a default description.
        type: parameters
      productType:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
  Issue:
    properties:
      attribute:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      severity:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  ListProductsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: parameters
      products:
        description: This is a default description.
        type: parameters
  Product:
    properties:
      contentLanguage:
        description: This is a default description.
        type: parameters
      issues:
        description: This is a default description.
        type: parameters
      manuallyDeletedAttributes:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      parent:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
      targetCountry:
        description: This is a default description.
        type: parameters
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