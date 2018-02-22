---
swagger: "2.0"
info:
  title: AWS ElastiCache API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeCacheEngineVersions&k=1:
    get:
      summary: ' Describe Cache Engine Versions '
      description: |-
        Returns a list of the available cache
                    engines and their versions
      operationId: describeCacheEngineVersions
      parameters:
      - in: query
        name: CacheParameterGroupFamily
        description: The name of a specific cache parameter group family to return
          details for
        type: string
      - in: query
        name: DefaultOnly
        description: If true, specifies that only the default version of the specified
          engine or engine            and major version combination is to be returned
        type: string
      - in: query
        name: Engine
        description: The cache engine to return
        type: string
      - in: query
        name: EngineVersion
        description: The cache engine version to return
        type: string
      - in: query
        name: Marker
        description: An optional marker returned from a prior request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - cache engine versions
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