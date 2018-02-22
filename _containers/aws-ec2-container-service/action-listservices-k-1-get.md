---
swagger: "2.0"
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListServices&k=1:
    get:
      summary: ' List Services '
      description: Lists the services that are running in a specified cluster
      operationId: listServices
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          that hosts the services to list
        type: string
      - in: query
        name: maxResults
        description: The maximum number of container instance results returned by                ListServices
          in paginated output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated                ListServices
          request where maxResults was used and the            results exceeded the
          value of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - services
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