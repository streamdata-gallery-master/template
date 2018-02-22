---
swagger: "2.0"
info:
  title: AWS CloudFront API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListInvalidations&k=1:
    get:
      summary: ' List Invalidations '
      description: Lists invalidation batches
      operationId: listInvalidations
      parameters:
      - in: query
        name: DhcpOptionsId
        description: The ID of the DHCP options set, or default to associate         no
          DHCP options with the VPC
        type: string
      - in: query
        name: DistributionId
        description: The distribution's ID
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Marker
        description: Use this parameter when paginating results to indicate where
          to begin in your list of      invalidation batches
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of invalidation batches that you want in the
          response      body
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
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