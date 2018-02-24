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
  /?Action=RestoreTableFromClusterSnapshot&k=1:
    get:
      summary: ' Restore Table From Cluster Snapshot '
      description: Creates a new table from a table in an Amazon Redshift cluster
        snapshot
      operationId: restoreTableFromClusterSnapshot
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The identifier of the Amazon Redshift cluster to restore the
          table to
        type: string
      - in: query
        name: NewTableName
        description: The name of the table to create as a result of the current request
        type: string
      - in: query
        name: SnapshotIdentifier
        description: The identifier of the snapshot to restore the table from
        type: string
      - in: query
        name: SourceDatabaseName
        description: The name of the source database that contains the table to restore
          from
        type: string
      - in: query
        name: SourceSchemaName
        description: The name of the source schema that contains the table to restore
          from
        type: string
      - in: query
        name: SourceTableName
        description: The name of the source table to restore from
        type: string
      - in: query
        name: TargetDatabaseName
        description: The name of the database to restore the table to
        type: string
      - in: query
        name: TargetSchemaName
        description: The name of the schema to restore the table to
        type: string
      responses:
        200:
          description: OK
      tags:
      - snapshots
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