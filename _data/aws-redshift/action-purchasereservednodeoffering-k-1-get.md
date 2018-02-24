---
swagger: "2.0"
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PurchaseReservedNodeOffering&k=1:
    get:
      summary: ' Purchase Reserved Node Offering '
      description: Allows you to purchase reserved nodes
      operationId: purchaseReservedNodeOffering
      parameters:
      - in: query
        name: NodeCount
        description: The number of reserved nodes that you want to purchase
        type: string
      - in: query
        name: ReservedNodeOfferingId
        description: The unique identifier of the reserved node offering you want
          to purchase
        type: string
      responses:
        200:
          description: OK
      tags:
      - reserved nodes
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