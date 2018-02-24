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
  /?Action=CreateMLModel&k=1:
    get:
      summary: ' Create M L Model '
      description: |-
        Creates a new MLModel using the DataSource and the recipe as
                    information sources
      operationId: createMLModel
      parameters:
      - in: query
        name: MLModelId
        description: A user-supplied ID that uniquely identifies the MLModel
        type: string
      - in: query
        name: MLModelName
        description: A user-supplied name or description of the MLModel
        type: string
      - in: query
        name: MLModelType
        description: The category of supervised learning that this MLModel will address
        type: string
      - in: query
        name: Parameters
        description: A list of the training parameters in the MLModel
        type: string
      - in: query
        name: Recipe
        description: The data recipe for creating the MLModel
        type: string
      - in: query
        name: RecipeUri
        description: The Amazon Simple Storage Service (Amazon S3) location and file
          name that contains the MLModel recipe
        type: string
      - in: query
        name: TrainingDataSourceId
        description: The DataSource that points to the training data
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