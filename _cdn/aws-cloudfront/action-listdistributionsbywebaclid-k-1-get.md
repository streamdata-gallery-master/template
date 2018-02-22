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
  /?Action=ListDistributionsByWebACLId&k=1:
    get:
      summary: ' List Distributions By Web A C L Id '
      description: List the distributions that are associated with a specified AWS
        WAF web ACL
      operationId: listDistributionsByWebACLId
      parameters:
      - in: query
        name: HostId.N
        description: The IDs of the Dedicated Hosts you want to release
        type: string
      - in: query
        name: Marker
        description: Use Marker and MaxItems to control pagination of results
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of distributions that you want CloudFront
          to return in the response body
        type: string
      - in: query
        name: WebACLId
        description: The ID of the AWS WAF web ACL that you want to list the associated
          distributions
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