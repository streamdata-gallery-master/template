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
  /?Action=GetChangeToken&k=1:
    get:
      summary: ' Get Change Token '
      description: 'Service: AWS WAFWhen you want to create, update, or delete AWS
        WAF objects, get a change token and include the change token in the create,
        update, or delete request'
      operationId: getChangeToken
      parameters:
      - in: query
        name: ChangeToken
        description: The ChangeToken that you used in the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - change token
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