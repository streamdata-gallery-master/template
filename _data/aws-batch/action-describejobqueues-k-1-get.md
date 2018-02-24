---
swagger: "2.0"
info:
  title: AWS Batch API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeJobQueues&k=1:
    get:
      summary: ' Describe Job Queues '
      description: Describes one or more of your job queues
      operationId: describeJobQueues
      parameters:
      - in: query
        name: jobQueues
        description: A list of up to 100 queue names or full queue Amazon Resource
          Name (ARN) entries
        type: string
      - in: query
        name: maxResults
        description: The maximum number of results returned by DescribeJobQueues in
          paginated         output
        type: string
      - in: query
        name: nextToken
        description: The nextToken value returned from a previous paginated            DescribeJobQueues
          request where maxResults was used and the         results exceeded the value
          of that parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - job queue
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