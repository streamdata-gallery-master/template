---
swagger: "2.0"
info:
  title: BigQuery
  description: A data platform for customers to create, manage, share and query data.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /bigquery/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{projectId}/datasets/{datasetId}/tables:
    post:
      summary: Create Table
      description: Creates a new, empty table in the dataset
      operationId: bigquery.tables.insert
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: datasetId
        description: Dataset ID of the new table
      - in: path
        name: projectId
        description: Project ID of the new table
      responses:
        200:
          description: OK
      tags:
      - table
definitions:
  BigtableColumn:
    properties:
      encoding:
        description: This is a default description.
        type: parameters
      fieldName:
        description: This is a default description.
        type: parameters
      onlyReadLatest:
        description: This is a default description.
        type: parameters
      qualifierEncoded:
        description: This is a default description.
        type: parameters
      qualifierString:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  BigtableColumnFamily:
    properties:
      columns:
        description: This is a default description.
        type: parameters
      encoding:
        description: This is a default description.
        type: parameters
      familyId:
        description: This is a default description.
        type: parameters
      onlyReadLatest:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  BigtableOptions:
    properties:
      columnFamilies:
        description: This is a default description.
        type: parameters
      ignoreUnspecifiedColumnFamilies:
        description: This is a default description.
        type: parameters
      readRowkeyAsString:
        description: This is a default description.
        type: parameters
  CsvOptions:
    properties:
      allowJaggedRows:
        description: This is a default description.
        type: parameters
      allowQuotedNewlines:
        description: This is a default description.
        type: parameters
      encoding:
        description: This is a default description.
        type: parameters
      fieldDelimiter:
        description: This is a default description.
        type: parameters
      quote:
        description: This is a default description.
        type: parameters
      skipLeadingRows:
        description: This is a default description.
        type: parameters
  Dataset:
    properties:
      access:
        description: This is a default description.
        type: parameters
      creationTime:
        description: This is a default description.
        type: parameters
      defaultTableExpirationMs:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      friendlyName:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      labels:
        description: This is a default description.
        type: parameters
      lastModifiedTime:
        description: This is a default description.
        type: parameters
  DatasetList:
    properties:
      datasets:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  DatasetReference:
    properties:
      datasetId:
        description: This is a default description.
        type: parameters
      projectId:
        description: This is a default description.
        type: parameters
  ErrorProto:
    properties:
      debugInfo:
        description: This is a default description.
        type: parameters
      location:
        description: This is a default description.
        type: parameters
      message:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
  ExplainQueryStage:
    properties:
      computeRatioAvg:
        description: This is a default description.
        type: parameters
      computeRatioMax:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      readRatioAvg:
        description: This is a default description.
        type: parameters
      readRatioMax:
        description: This is a default description.
        type: parameters
      recordsRead:
        description: This is a default description.
        type: parameters
      recordsWritten:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      steps:
        description: This is a default description.
        type: parameters
  ExplainQueryStep:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      substeps:
        description: This is a default description.
        type: parameters
  ExternalDataConfiguration:
    properties:
      autodetect:
        description: This is a default description.
        type: parameters
      compression:
        description: This is a default description.
        type: parameters
      ignoreUnknownValues:
        description: This is a default description.
        type: parameters
      maxBadRecords:
        description: This is a default description.
        type: parameters
      sourceFormat:
        description: This is a default description.
        type: parameters
      sourceUris:
        description: This is a default description.
        type: parameters
  GetQueryResultsResponse:
    properties:
      cacheHit:
        description: This is a default description.
        type: parameters
      errors:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      jobComplete:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      numDmlAffectedRows:
        description: This is a default description.
        type: parameters
      pageToken:
        description: This is a default description.
        type: parameters
      rows:
        description: This is a default description.
        type: parameters
      totalBytesProcessed:
        description: This is a default description.
        type: parameters
      totalRows:
        description: This is a default description.
        type: parameters
  GoogleSheetsOptions:
    properties:
      skipLeadingRows:
        description: This is a default description.
        type: parameters
  Job:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      user_email:
        description: This is a default description.
        type: parameters
  JobCancelResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
  JobConfiguration:
    properties:
      dryRun:
        description: This is a default description.
        type: parameters
      labels:
        description: This is a default description.
        type: parameters
  JobConfigurationExtract:
    properties:
      compression:
        description: This is a default description.
        type: parameters
      destinationFormat:
        description: This is a default description.
        type: parameters
      destinationUri:
        description: This is a default description.
        type: parameters
      destinationUris:
        description: This is a default description.
        type: parameters
      fieldDelimiter:
        description: This is a default description.
        type: parameters
      printHeader:
        description: This is a default description.
        type: parameters
  JobConfigurationLoad:
    properties:
      allowJaggedRows:
        description: This is a default description.
        type: parameters
      allowQuotedNewlines:
        description: This is a default description.
        type: parameters
      autodetect:
        description: This is a default description.
        type: parameters
      createDisposition:
        description: This is a default description.
        type: parameters
      encoding:
        description: This is a default description.
        type: parameters
      fieldDelimiter:
        description: This is a default description.
        type: parameters
      ignoreUnknownValues:
        description: This is a default description.
        type: parameters
      maxBadRecords:
        description: This is a default description.
        type: parameters
      nullMarker:
        description: This is a default description.
        type: parameters
      projectionFields:
        description: This is a default description.
        type: parameters
  JobConfigurationQuery:
    properties:
      allowLargeResults:
        description: This is a default description.
        type: parameters
      createDisposition:
        description: This is a default description.
        type: parameters
      flattenResults:
        description: This is a default description.
        type: parameters
      maximumBillingTier:
        description: This is a default description.
        type: parameters
      maximumBytesBilled:
        description: This is a default description.
        type: parameters
      parameterMode:
        description: This is a default description.
        type: parameters
      preserveNulls:
        description: This is a default description.
        type: parameters
      priority:
        description: This is a default description.
        type: parameters
      query:
        description: This is a default description.
        type: parameters
      queryParameters:
        description: This is a default description.
        type: parameters
  JobConfigurationTableCopy:
    properties:
      createDisposition:
        description: This is a default description.
        type: parameters
      sourceTables:
        description: This is a default description.
        type: parameters
      writeDisposition:
        description: This is a default description.
        type: parameters
  JobList:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      jobs:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  JobReference:
    properties:
      jobId:
        description: This is a default description.
        type: parameters
      projectId:
        description: This is a default description.
        type: parameters
  JobStatistics:
    properties:
      creationTime:
        description: This is a default description.
        type: parameters
      endTime:
        description: This is a default description.
        type: parameters
      startTime:
        description: This is a default description.
        type: parameters
      totalBytesProcessed:
        description: This is a default description.
        type: parameters
  JobStatistics2:
    properties:
      billingTier:
        description: This is a default description.
        type: parameters
      cacheHit:
        description: This is a default description.
        type: parameters
      numDmlAffectedRows:
        description: This is a default description.
        type: parameters
      queryPlan:
        description: This is a default description.
        type: parameters
      referencedTables:
        description: This is a default description.
        type: parameters
      statementType:
        description: This is a default description.
        type: parameters
      totalBytesBilled:
        description: This is a default description.
        type: parameters
      totalBytesProcessed:
        description: This is a default description.
        type: parameters
      undeclaredQueryParameters:
        description: This is a default description.
        type: parameters
  JobStatistics3:
    properties:
      inputFileBytes:
        description: This is a default description.
        type: parameters
      inputFiles:
        description: This is a default description.
        type: parameters
      outputBytes:
        description: This is a default description.
        type: parameters
      outputRows:
        description: This is a default description.
        type: parameters
  JobStatistics4:
    properties:
      destinationUriFileCounts:
        description: This is a default description.
        type: parameters
  JobStatus:
    properties:
      errors:
        description: This is a default description.
        type: parameters
      state:
        description: This is a default description.
        type: parameters
  ProjectList:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      projects:
        description: This is a default description.
        type: parameters
      totalItems:
        description: This is a default description.
        type: parameters
  ProjectReference:
    properties:
      projectId:
        description: This is a default description.
        type: parameters
  QueryParameter:
    properties:
      name:
        description: This is a default description.
        type: parameters
  QueryParameterType:
    properties:
      structTypes:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  QueryParameterValue:
    properties:
      arrayValues:
        description: This is a default description.
        type: parameters
      structValues:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  QueryRequest:
    properties:
      dryRun:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      maxResults:
        description: This is a default description.
        type: parameters
      parameterMode:
        description: This is a default description.
        type: parameters
      preserveNulls:
        description: This is a default description.
        type: parameters
      query:
        description: This is a default description.
        type: parameters
      queryParameters:
        description: This is a default description.
        type: parameters
      timeoutMs:
        description: This is a default description.
        type: parameters
      useLegacySql:
        description: This is a default description.
        type: parameters
      useQueryCache:
        description: This is a default description.
        type: parameters
  QueryResponse:
    properties:
      cacheHit:
        description: This is a default description.
        type: parameters
      errors:
        description: This is a default description.
        type: parameters
      jobComplete:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      numDmlAffectedRows:
        description: This is a default description.
        type: parameters
      pageToken:
        description: This is a default description.
        type: parameters
      rows:
        description: This is a default description.
        type: parameters
      totalBytesProcessed:
        description: This is a default description.
        type: parameters
      totalRows:
        description: This is a default description.
        type: parameters
  Streamingbuffer:
    properties:
      estimatedBytes:
        description: This is a default description.
        type: parameters
      estimatedRows:
        description: This is a default description.
        type: parameters
      oldestEntryTime:
        description: This is a default description.
        type: parameters
  Table:
    properties:
      creationTime:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      expirationTime:
        description: This is a default description.
        type: parameters
      friendlyName:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      labels:
        description: This is a default description.
        type: parameters
      lastModifiedTime:
        description: This is a default description.
        type: parameters
      location:
        description: This is a default description.
        type: parameters
  TableCell:
    properties: []
  TableDataInsertAllRequest:
    properties:
      ignoreUnknownValues:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      rows:
        description: This is a default description.
        type: parameters
      skipInvalidRows:
        description: This is a default description.
        type: parameters
      templateSuffix:
        description: This is a default description.
        type: parameters
  TableDataInsertAllResponse:
    properties:
      insertErrors:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  TableDataList:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      pageToken:
        description: This is a default description.
        type: parameters
      rows:
        description: This is a default description.
        type: parameters
      totalRows:
        description: This is a default description.
        type: parameters
  TableFieldSchema:
    properties:
      description:
        description: This is a default description.
        type: parameters
      fields:
        description: This is a default description.
        type: parameters
      mode:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  TableList:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      tables:
        description: This is a default description.
        type: parameters
      totalItems:
        description: This is a default description.
        type: parameters
  TableReference:
    properties:
      datasetId:
        description: This is a default description.
        type: parameters
      projectId:
        description: This is a default description.
        type: parameters
      tableId:
        description: This is a default description.
        type: parameters
  TableRow:
    properties:
      f:
        description: This is a default description.
        type: parameters
  TableSchema:
    properties:
      fields:
        description: This is a default description.
        type: parameters
  TimePartitioning:
    properties:
      expirationMs:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  UserDefinedFunctionResource:
    properties:
      inlineCode:
        description: This is a default description.
        type: parameters
      resourceUri:
        description: This is a default description.
        type: parameters
  ViewDefinition:
    properties:
      query:
        description: This is a default description.
        type: parameters
      useLegacySql:
        description: This is a default description.
        type: parameters
      userDefinedFunctionResources:
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