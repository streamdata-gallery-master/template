---
swagger: "2.0"
info:
  title: The Noun Project
  description: The Noun Project is a website that aggregates and catalogs symbols
    that are created and uploaded by graphic designers around the world. Based in
    Los Angeles, the project functions both as a resource for people in search of
    typographic symbols and a design history of the genre.
  version: v1
host: api.thenounproject.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collection/{id}/icons:
    get:
      summary: Get collection icons by id
      description: Returns a list of icons associated with a collection
      operationId: getCollectionIconsById
      parameters:
      - in: path
        name: id
        description: Collection id
      - in: query
        name: limit
        description: Maximum number of results
      - in: query
        name: offset
        description: Number of results to displace or skip over
      - in: query
        name: page
        description: Number of results of limit length to displace or skip over
      responses:
        200:
          description: OK
      tags:
      - images
      - collections
      - icons
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