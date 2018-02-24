---
swagger: "2.0"
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListTopicRules&k=1:
    get:
      summary: ' List Topic Rules '
      description: Lists the rules for the specific topic
      operationId: listTopicRules
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of results to return
        type: string
      - in: query
        name: nextToken
        description: A token used to retrieve the next value
        type: string
      - in: query
        name: ruleDisabled
        description: Specifies whether the rule is disabled
        type: string
      - in: query
        name: topic
        description: The topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - topic rules
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