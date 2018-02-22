---
swagger: "2.0"
info:
  title: APIs Discovery Service
  description: Provides information about other Google APIs, such as what APIs are
    available, the resource, and method details for each API.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /discovery/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apis/{api}/{version}/rest:
    get:
      summary: Get API Description
      description: Retrieve the description of a particular version of an api
      operationId: discovery.apis.getRest
      parameters:
      - in: path
        name: api
        description: The name of the API
      - in: path
        name: version
        description: The version of the API
      responses:
        200:
          description: OK
      tags:
      - api
definitions:
  DirectoryList:
    properties:
      discoveryVersion:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  JsonSchema:
    properties:
      $ref:
        description: This is a default description.
        type: parameters
      annotations:
        description: This is a default description.
        type: parameters
      default:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      enum:
        description: This is a default description.
        type: parameters
      enumDescriptions:
        description: This is a default description.
        type: parameters
      format:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      location:
        description: This is a default description.
        type: parameters
      maximum:
        description: This is a default description.
        type: parameters
  RestDescription:
    properties:
      auth:
        description: This is a default description.
        type: parameters
      basePath:
        description: This is a default description.
        type: parameters
      baseUrl:
        description: This is a default description.
        type: parameters
      batchPath:
        description: This is a default description.
        type: parameters
      canonicalName:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      discoveryVersion:
        description: This is a default description.
        type: parameters
      documentationLink:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      exponentialBackoffDefault:
        description: This is a default description.
        type: parameters
  RestMethod:
    properties:
      description:
        description: This is a default description.
        type: parameters
      etagRequired:
        description: This is a default description.
        type: parameters
      httpMethod:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      mediaUpload:
        description: This is a default description.
        type: parameters
      parameterOrder:
        description: This is a default description.
        type: parameters
      parameters:
        description: This is a default description.
        type: parameters
      path:
        description: This is a default description.
        type: parameters
      request:
        description: This is a default description.
        type: parameters
      response:
        description: This is a default description.
        type: parameters
  RestResource:
    properties:
      methods:
        description: This is a default description.
        type: parameters
      resources:
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