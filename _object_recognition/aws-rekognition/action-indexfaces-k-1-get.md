---
swagger: "2.0"
info:
  title: AWS Rekognition API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=IndexFaces&k=1:
    get:
      summary: ' Index Faces '
      description: Detects faces in the input image and adds them to the specified
        collection
      operationId: indexFaces
      parameters:
      - in: query
        name: CollectionId
        description: ID of an existing collection to which you want to add the faces
          that are detected in the      input images
        type: string
      - in: query
        name: DetectionAttributes
        description: (Optional) Returns detailed attributes of indexed faces
        type: string
      - in: query
        name: ExternalImageId
        description: ID you want to assign to all the faces detected in the image
        type: string
      - in: query
        name: Image
        description: Provides the source image either as bytes or an S3 object
        type: string
      responses:
        200:
          description: OK
      tags:
      - faces
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