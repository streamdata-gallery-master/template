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
  /?Action=GetXssMatchSet&k=1:
    get:
      summary: ' Get Xss Match Set '
      description: 'Service: AWS WAFReturns the'
      operationId: getXssMatchSet
      parameters:
      - in: query
        name: XssMatchSetId
        description: The XssMatchSetId of the XssMatchSet that you want to get
        type: string
      responses:
        200:
          description: OK
      tags:
      - xss match set
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