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
  /?Action=SearchFaces&k=1:
    get:
      summary: ' Search Faces '
      description: For a given input face ID, searches for matching faces in the collection
        the face belongs to
      operationId: searchFaces
      parameters:
      - in: query
        name: CollectionId
        description: ID of the collection the face belongs to
        type: string
      - in: query
        name: FaceId
        description: ID of a face to find matches for in the collection
        type: string
      - in: query
        name: FaceMatchThreshold
        description: Optional value specifying the minimum confidence in the face
          match to return
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