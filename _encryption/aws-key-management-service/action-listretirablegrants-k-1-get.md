---
swagger: "2.0"
info:
  title: AWS Key Management Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListRetirableGrants&k=1:
    get:
      summary: ' List Retirable Grants '
      description: |-
        Returns a list of all grants for which the grant's RetiringPrincipal
              matches the one specified
      operationId: listRetirableGrants
      parameters:
      - in: query
        name: Limit
        description: When paginating results, specify the maximum number of items
          to return in the response
        type: string
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only in a
          subsequent request after      you receive a response with truncated results
        type: string
      - in: query
        name: RetiringPrincipal
        description: The retiring principal for which to list grants
        type: string
      responses:
        200:
          description: OK
      tags:
      - grants
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