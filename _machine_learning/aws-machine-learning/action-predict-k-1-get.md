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
  /?Action=Predict&k=1:
    get:
      summary: ' Predict '
      description: Generates a prediction for the observation using the specified
        ML Model
      operationId: predict
      parameters:
      - in: query
        name: MLModelId
        description: A unique identifier of the MLModel
        type: string
      - in: query
        name: PredictEndpoint
        description: 'Type: String'
        type: string
      - in: query
        name: Record
        description: A map of variable name-value pairs that represent an observation
        type: string
      responses:
        200:
          description: OK
      tags:
      - predict
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