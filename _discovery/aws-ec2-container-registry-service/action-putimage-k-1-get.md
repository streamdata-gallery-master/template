---
swagger: "2.0"
info:
  title: AWS EC2 Container Registry API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=PutImage&k=1:
    get:
      summary: ' Put Image '
      description: Creates or updates the image manifest and tags associated with
        an image
      operationId: putImage
      parameters:
      - in: query
        name: imageManifest
        description: The image manifest corresponding to the image to be uploaded
        type: string
      - in: query
        name: imageTag
        description: The tag to associate with the image
        type: string
      - in: query
        name: registryId
        description: The AWS account ID associated with the registry that contains
          the repository in which to put the image
        type: string
      - in: query
        name: repositoryName
        description: The name of the repository in which to put the image
        type: string
      responses:
        200:
          description: OK
      tags:
      - images
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