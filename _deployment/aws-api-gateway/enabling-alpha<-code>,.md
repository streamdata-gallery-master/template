---
swagger: "2.0"
info:
  title: AWS API Gateway API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  enabling:
    alpha</code>,:
      summary: Stage Create
      description: Creates a new stage, as represented by a Stage instance, in a pre-existing
        Deployment of an API
      operationId: stageCreate
      parameters:
      - in: header
        name: '&quot;cacheClusterEnabled&quot;'
        type: string
      - in: header
        name: '&quot;cacheClusterSize&quot;'
        type: string
      - in: header
        name: '&quot;deploymentId&quot;'
        type: string
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: '&quot;stageName&quot;'
        type: string
      - in: header
        name: '&quot;sv_1&quot;'
        type: string
      - in: header
        name: '&quot;sv_2&quot;'
        type: string
      - in: header
        name: '&quot;variables&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: query
        name: DryRun
        description: "Checks whether you have the required permissions for the action,
          without actually making the request, \t    and provides an error response"
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: header
        name: Host
        type: string
      - in: query
        name: InstanceId.N
        description: One or more instance IDs
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of results to return for the request in a
          single page
        type: string
      - in: query
        name: NextToken
        description: The token to retrieve the next page of results
        type: string
      - in: header
        name: X-Amz-Date
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