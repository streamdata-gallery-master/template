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
  /?Action=GetBatchPrediction&k=1:
    get:
      summary: ' Get Batch Prediction '
      description: |-
        Returns a BatchPrediction that includes detailed metadata, status, and data file information for a
                    Batch Prediction request
      operationId: getBatchPrediction
      parameters:
      - in: query
        name: BatchPredictionId
        description: An ID assigned to the BatchPrediction at creation
        type: string
      responses:
        200:
          description: OK
      tags:
      - batches
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