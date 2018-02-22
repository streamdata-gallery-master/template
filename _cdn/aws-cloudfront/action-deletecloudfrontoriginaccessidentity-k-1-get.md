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
  /?Action=DeleteCloudFrontOriginAccessIdentity&k=1:
    get:
      summary: ' Delete Cloud Front Origin Access Identity '
      description: Delete an origin access identity
      operationId: deleteCloudFrontOriginAccessIdentity
      parameters:
      - in: query
        name: Id
        description: The origin access identity's ID
        type: string
      - in: query
        name: If-Match
        description: The value of the ETag header you received from a previous GET      or
          PUT request
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