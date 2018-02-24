---
swagger: "2.0"
info:
  title: Google Storage Transfer
  description: Transfers data from external data sources to a Google Cloud Storage
    bucket or between Google Cloud Storage buckets.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: storagetransfer.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:cancel:
    post:
      summary: Cancel Transfer Operation
      description: Cancels a transfer
      operationId: storagetransfer.transferOperations.cancel
      parameters:
      - in: path
        name: name
        description: The name of the operation resource to be cancelled
      responses:
        200:
          description: OK
      tags:
      - operation
definitions:
  AwsAccessKey:
    properties:
      accessKeyId:
        description: This is a default description.
        type: parameters
      secretAccessKey:
        description: This is a default description.
        type: parameters
  AwsS3Data:
    properties:
      bucketName:
        description: This is a default description.
        type: parameters
  Date:
    properties:
      day:
        description: This is a default description.
        type: parameters
      month:
        description: This is a default description.
        type: parameters
      year:
        description: This is a default description.
        type: parameters
  ErrorLogEntry:
    properties:
      errorDetails:
        description: This is a default description.
        type: parameters
      url:
        description: This is a default description.
        type: parameters
  ErrorSummary:
    properties:
      errorCode:
        description: This is a default description.
        type: parameters
      errorCount:
        description: This is a default description.
        type: parameters
      errorLogEntries:
        description: This is a default description.
        type: parameters
  GcsData:
    properties:
      bucketName:
        description: This is a default description.
        type: parameters
  GoogleServiceAccount:
    properties:
      accountEmail:
        description: This is a default description.
        type: parameters
  HttpData:
    properties:
      listUrl:
        description: This is a default description.
        type: parameters
  ListOperationsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: parameters
      operations:
        description: This is a default description.
        type: parameters
  ListTransferJobsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: parameters
      transferJobs:
        description: This is a default description.
        type: parameters
  ObjectConditions:
    properties:
      excludePrefixes:
        description: This is a default description.
        type: parameters
      includePrefixes:
        description: This is a default description.
        type: parameters
      maxTimeElapsedSinceLastModification:
        description: This is a default description.
        type: parameters
      minTimeElapsedSinceLastModification:
        description: This is a default description.
        type: parameters
  Operation:
    properties:
      done:
        description: This is a default description.
        type: parameters
      metadata:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      response:
        description: This is a default description.
        type: parameters
  Schedule:
    properties: []
  Status:
    properties:
      code:
        description: This is a default description.
        type: parameters
      details:
        description: This is a default description.
        type: parameters
      message:
        description: This is a default description.
        type: parameters
  TimeOfDay:
    properties:
      hours:
        description: This is a default description.
        type: parameters
      minutes:
        description: This is a default description.
        type: parameters
      nanos:
        description: This is a default description.
        type: parameters
      seconds:
        description: This is a default description.
        type: parameters
  TransferCounters:
    properties:
      bytesCopiedToSink:
        description: This is a default description.
        type: parameters
      bytesDeletedFromSink:
        description: This is a default description.
        type: parameters
      bytesDeletedFromSource:
        description: This is a default description.
        type: parameters
      bytesFailedToDeleteFromSink:
        description: This is a default description.
        type: parameters
      bytesFoundFromSource:
        description: This is a default description.
        type: parameters
      bytesFoundOnlyFromSink:
        description: This is a default description.
        type: parameters
      bytesFromSourceFailed:
        description: This is a default description.
        type: parameters
      bytesFromSourceSkippedBySync:
        description: This is a default description.
        type: parameters
      objectsCopiedToSink:
        description: This is a default description.
        type: parameters
      objectsDeletedFromSink:
        description: This is a default description.
        type: parameters
  TransferJob:
    properties:
      creationTime:
        description: This is a default description.
        type: parameters
      deletionTime:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      lastModificationTime:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      projectId:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
  TransferOperation:
    properties:
      endTime:
        description: This is a default description.
        type: parameters
      errorBreakdowns:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      projectId:
        description: This is a default description.
        type: parameters
      startTime:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      transferJobName:
        description: This is a default description.
        type: parameters
  TransferOptions:
    properties:
      deleteObjectsFromSourceAfterTransfer:
        description: This is a default description.
        type: parameters
      deleteObjectsUniqueInSink:
        description: This is a default description.
        type: parameters
      overwriteObjectsAlreadyExistingInSink:
        description: This is a default description.
        type: parameters
  TransferSpec:
    properties: []
  UpdateTransferJobRequest:
    properties:
      projectId:
        description: This is a default description.
        type: parameters
      updateTransferJobFieldMask:
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