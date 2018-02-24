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
  /?Action=DescribeProductAsAdmin&k=1:
    get:
      summary: ' Describe Product As Admin '
      description: |-
        Retrieves information about a specified product, run with administrator
                 access
      operationId: describeProductAsAdmin
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The identifier of the product for which to retrieve information
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