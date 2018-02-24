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
  /?Action=GetMLModel&k=1:
    get:
      summary: ' Get M L Model '
      description: Returns an MLModel that includes detailed metadata, data source
        information, and the current status of the MLModel
      operationId: getMLModel
      parameters:
      - in: query
        name: MLModelId
        description: The ID assigned to the MLModel at creation
        type: string
      - in: query
        name: Verbose
        description: Specifies whether the GetMLModel operation should return Recipe
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