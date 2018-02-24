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
  /?Action=DetectFaces&k=1:
    get:
      summary: ' Detect Faces '
      description: Detects faces within an image (JPEG or PNG) that is provided as
        input
      operationId: detectFaces
      parameters:
      - in: query
        name: Attributes
        description: A list of facial attributes you would like to be returned
        type: string
      - in: query
        name: Image
        description: The image in which you want to detect faces
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