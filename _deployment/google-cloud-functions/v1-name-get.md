---
swagger: "2.0"
info:
  title: Google Cloud Functions
  description: API for managing lightweight user-provided functions executed in response
    to events.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudfunctions.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:
    get:
      summary: Get Location
      description: Get information about a location
      operationId: cloudfunctions.projects.locations.get
      parameters:
      - in: path
        name: name
        description: Resource name for the location
      responses:
        200:
          description: OK
      tags:
      - location
definitions:
  Location:
    properties:
      labels:
        description: This is a default description.
        type: parameters
      locationId:
        description: This is a default description.
        type: parameters
      metadata:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
  OperationMetadataV1Beta2:
    properties:
      request:
        description: This is a default description.
        type: parameters
      target:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
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