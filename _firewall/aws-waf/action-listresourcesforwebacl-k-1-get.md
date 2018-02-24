---
swagger: "2.0"
info:
  title: AWS WAF API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListResourcesForWebACL&k=1:
    get:
      summary: ' List Resources For Web ACL'
      description: 'Service: AWS WAF RegionalReturns an array of resources associated
        with the specified web ACL'
      operationId: listResourcesForWebACL
      parameters:
      - in: query
        name: WebACLId
        description: The unique identifier (ID) of the web ACL for which to list the
          associated resources
        type: string
      responses:
        200:
          description: OK
      tags:
      - web acl
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