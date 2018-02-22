---
swagger: "2.0"
info:
  title: AWS Elastic MapReduce API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListClusters&k=1:
    get:
      summary: ' List Clusters '
      description: Provides the status of all clusters visible to this AWS account
      operationId: listClusters
      parameters:
      - in: query
        name: ClusterStates
        description: The cluster state filters to apply when listing clusters
        type: string
      - in: query
        name: CreatedAfter
        description: The creation date and time beginning value filter for listing
          clusters
        type: string
      - in: query
        name: CreatedBefore
        description: The creation date and time end value filter for listing clusters
        type: string
      - in: query
        name: Marker
        description: The pagination token that indicates the next set of results to
          retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - clusters
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