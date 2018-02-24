---
swagger: "2.0"
info:
  title: Enterprise License Manager
  description: Views and manages licenses for your domain.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /apps/licensing/v1/product
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{productId}/sku/{skuId}/user/{userId}:
    delete:
      summary: Revoke License
      description: Revoke License
      operationId: licensing.licenseAssignments.delete
      parameters:
      - in: path
        name: productId
        description: Name for product
      - in: path
        name: skuId
        description: Name for sku
      - in: path
        name: userId
        description: email id or unique Id of the user
      responses:
        200:
          description: OK
      tags:
      - license
definitions:
  LicenseAssignment:
    properties:
      etags:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
      productName:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      skuId:
        description: This is a default description.
        type: parameters
      skuName:
        description: This is a default description.
        type: parameters
      userId:
        description: This is a default description.
        type: parameters
  LicenseAssignmentInsert:
    properties:
      userId:
        description: This is a default description.
        type: parameters
  LicenseAssignmentList:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
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