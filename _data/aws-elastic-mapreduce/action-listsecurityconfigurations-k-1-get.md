---
swagger: "2.0"
info:
  title: AWS Elastic MapReduce API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListSecurityConfigurations&k=1:
    get:
      summary: ' List Security Configurations '
      description: Lists all the security configurations visible to this account,
        providing their creation dates and times, and their names
      operationId: listSecurityConfigurations
      parameters:
      - in: query
        name: Marker
        description: The pagination token that indicates the set of results to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - security configurations
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