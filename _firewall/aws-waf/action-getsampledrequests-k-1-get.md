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
  /?Action=GetSampledRequests&k=1:
    get:
      summary: ' Get Sampled Requests '
      description: 'Service: AWS WAFGets detailed information about a specified number
        of requests--a sample--that AWS WAF randomly selects from among the first
        5,000 requests that your AWS resource received during a time range that you
        choose'
      operationId: getSampledRequests
      parameters:
      - in: query
        name: MaxItems
        description: "The number of requests that you want AWS WAF to return from
          among the first 5,000 requests that your AWS resource received\t\t\tduring
          the time range"
        type: string
      - in: query
        name: RuleId
        description: 'RuleId is one of two values:'
        type: string
      - in: query
        name: TimeWindow
        description: "The start date and time and the end date and time of the range
          for which you want GetSampledRequests to return a \t\t    \tsample of requests"
        type: string
      - in: query
        name: WebAclId
        description: The WebACLId of the WebACL for which you want GetSampledRequests
          to return a sample of requests
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