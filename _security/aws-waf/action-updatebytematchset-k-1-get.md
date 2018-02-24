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
  /?Action=UpdateByteMatchSet&k=1:
    get:
      summary: ' Update Byte Match Set '
      description: 'Service: AWS WAFInserts or deletes'
      operationId: updateByteMatchSet
      parameters:
      - in: query
        name: ByteMatchSetId
        description: The ByteMatchSetId of the ByteMatchSet that you want to update
        type: string
      - in: query
        name: ChangeToken
        description: The value returned by the most recent call to GetChangeToken
        type: string
      - in: query
        name: Updates
        description: An array of ByteMatchSetUpdate objects that you want to insert
          into or delete from a ByteMatchSet
        type: string
      responses:
        200:
          description: OK
      tags:
      - byte match set
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