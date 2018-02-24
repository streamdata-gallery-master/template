---
swagger: "2.0"
info:
  title: Google App State
  description: The Google App State API.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /appstate/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /states:
    get:
      summary: Get State Keys
      description: Lists all the states keys, and optionally the state data
      operationId: appstate.states.list
      parameters:
      - in: query
        name: includeData
        description: Whether to include the full data in addition to the version number
      responses:
        200:
          description: OK
      tags:
      - application state
definitions:
  GetResponse:
    properties:
      currentStateVersion:
        description: This is a default description.
        type: post
      data:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      stateKey:
        description: This is a default description.
        type: post
  ListResponse:
    properties:
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      maximumKeyCount:
        description: This is a default description.
        type: post
  UpdateRequest:
    properties:
      data:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  WriteResult:
    properties:
      currentStateVersion:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      stateKey:
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