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
  /?Action=AssociateWebACL&k=1:
    get:
      summary: ' Associate Web ACL '
      description: 'Service: AWS WAF RegionalAssociates a web ACL with a resource'
      operationId: associateWebACL
      parameters:
      - in: query
        name: ResourceArn
        description: The ARN (Amazon Resource Name) of the resource to be protected
        type: string
      - in: query
        name: WebACLId
        description: A unique identifier (ID) for the web ACL
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