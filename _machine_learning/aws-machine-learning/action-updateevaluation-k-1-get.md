---
swagger: "2.0"
info:
  title: AWS Machine Learning API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateEvaluation&k=1:
    get:
      summary: ' Update Evaluation '
      description: Updates the EvaluationName of an Evaluation
      operationId: updateEvaluation
      parameters:
      - in: query
        name: EvaluationId
        description: The ID assigned to the Evaluation during creation
        type: string
      - in: query
        name: EvaluationName
        description: A new user-supplied name or description of the Evaluation that
          will replace the current content
        type: string
      responses:
        200:
          description: OK
      tags:
      - evaluations
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