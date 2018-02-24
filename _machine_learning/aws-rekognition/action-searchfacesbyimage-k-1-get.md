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
  /?Action=SearchFacesByImage&k=1:
    get:
      summary: ' Search Faces By Image '
      description: |-
        For a given input image, first detects the largest face in the image, and
              then searches the specified collection for matching faces
      operationId: searchFacesByImage
      parameters:
      - in: query
        name: CollectionId
        description: ID of the collection to search
        type: string
      - in: query
        name: FaceMatchThreshold
        description: (Optional) Specifies the minimum confidence in the face match
          to return
        type: string
      - in: query
        name: Image
        description: Provides the source image either as bytes or an S3 object
        type: string
      - in: query
        name: MaxFaces
        description: Maximum number of faces to return
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