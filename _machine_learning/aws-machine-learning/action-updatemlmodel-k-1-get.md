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
  /?Action=UpdateMLModel&k=1:
    get:
      summary: ' Update M L Model '
      description: Updates the MLModelName and the ScoreThreshold of an MLModel
      operationId: updateMLModel
      parameters:
      - in: query
        name: MLModelId
        description: The ID assigned to the MLModel during creation
        type: string
      - in: query
        name: MLModelName
        description: A user-supplied name or description of the MLModel
        type: string
      - in: query
        name: ScoreThreshold
        description: The ScoreThreshold used in binary classification MLModel that
          marks the boundary between a positive prediction and a negative prediction
        type: string
      responses:
        200:
          description: OK
      tags:
      - models
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