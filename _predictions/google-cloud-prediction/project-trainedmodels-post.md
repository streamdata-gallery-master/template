---
swagger: "2.0"
info:
  title: Prediction
  description: Lets you access a cloud hosted machine learning service that makes
    it easy to build smart apps
  contact:
    name: Google
    url: https://google.com
  version: v1.6
host: www.googleapis.com
basePath: /prediction/v1.6/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/trainedmodels:
    post:
      summary: Train Model
      description: Train a Prediction API model
      operationId: prediction.trainedmodels.insert
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: The project associated with the model
      responses:
        200:
          description: OK
      tags:
      - model
definitions:
  Analyze:
    properties:
      dataDescription:
        description: This is a default description.
        type: post
      errors:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      modelDescription:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  Input:
    properties:
      input:
        description: This is a default description.
        type: post
  Insert:
    properties:
      id:
        description: This is a default description.
        type: post
      modelType:
        description: This is a default description.
        type: post
      sourceModel:
        description: This is a default description.
        type: post
      storageDataLocation:
        description: This is a default description.
        type: post
      storagePMMLLocation:
        description: This is a default description.
        type: post
      storagePMMLModelLocation:
        description: This is a default description.
        type: post
      trainingInstances:
        description: This is a default description.
        type: post
      utility:
        description: This is a default description.
        type: post
  Insert2:
    properties:
      created:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      modelInfo:
        description: This is a default description.
        type: post
      modelType:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
      storageDataLocation:
        description: This is a default description.
        type: post
      storagePMMLLocation:
        description: This is a default description.
        type: post
      storagePMMLModelLocation:
        description: This is a default description.
        type: post
      trainingComplete:
        description: This is a default description.
        type: post
  List:
    properties:
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  Output:
    properties:
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      outputLabel:
        description: This is a default description.
        type: post
      outputMulti:
        description: This is a default description.
        type: post
      outputValue:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  Update:
    properties:
      csvInstance:
        description: This is a default description.
        type: post
      output:
        description: This is a default description.
        type: post
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