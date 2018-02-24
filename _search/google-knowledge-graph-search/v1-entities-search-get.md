---
swagger: "2.0"
info:
  title: Knowledge Graph Search
  description: Searches the Google Knowledge Graph for entities.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: kgsearch.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/entities:search:
    get:
      summary: Search Knowledge Graph
      description: Searches Knowledge Graph for entities that match the constraints
      operationId: kgsearch.entities.search
      parameters:
      - in: query
        name: ids
        description: The list of entity id to be used for search instead of query
          string
      - in: query
        name: indent
        description: Enables indenting of json results
      - in: query
        name: languages
        description: |-
          The list of language codes (defined in ISO 693) to run the query with,
          e
      - in: query
        name: limit
        description: Limits the number of entities to be returned
      - in: query
        name: prefix
        description: Enables prefix match against names and aliases of entities
      - in: query
        name: query
        description: The literal query string for search
      - in: query
        name: types
        description: Restricts returned entities with these types, e
      responses:
        200:
          description: OK
      tags:
      - knowledge graph
definitions:
  SearchResponse:
    properties:
      itemListElement:
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