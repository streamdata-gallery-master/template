---
swagger: "2.0"
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteCluster&k=1:
    get:
      summary: ' Delete Cluster '
      description: Deletes a previously provisioned cluster
      operationId: deleteCluster
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the cluster to be deleted
        type: string
      - in: query
        name: FinalClusterSnapshotIdentifier
        description: The identifier of the final snapshot that is to be created immediately
          before            deleting the cluster
        type: string
      - in: query
        name: SkipFinalClusterSnapshot
        description: Determines whether a final snapshot of the cluster is created
          before Amazon Redshift            deletes the cluster
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