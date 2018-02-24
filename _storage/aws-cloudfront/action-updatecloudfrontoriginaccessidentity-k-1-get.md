---
swagger: "2.0"
info:
  title: AWS CloudFront API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateCloudFrontOriginAccessIdentity&k=1:
    get:
      summary: ' Update Cloud Front Origin Access Identity '
      description: Update an origin access identity
      operationId: updateCloudFrontOriginAccessIdentity
      parameters:
      - in: query
        name: Description
        description: A description for the EBS snapshot
        type: string
      - in: query
        name: DestinationRegion
        description: The destination region to use in the PresignedUrl parameter of
          a snapshot copy      operation
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: Encrypted
        description: Specifies whether the destination snapshot should be encrypted
        type: string
      - in: query
        name: Id
        description: The identity's id
        type: string
      - in: query
        name: If-Match
        description: The value of the ETag header that you received when retrieving
          the      identity's configuration
        type: string
      - in: query
        name: KmsKeyId
        description: The full ARN of the AWS Key Management Service (AWS KMS) CMK
          to use when creating the snapshot copy
        type: string
      - in: query
        name: PresignedUrl
        description: The pre-signed URL that facilitates copying an encrypted snapshot
        type: string
      - in: query
        name: SourceRegion
        description: The ID of the region that contains the snapshot to be copied
        type: string
      - in: query
        name: SourceSnapshotId
        description: The ID of the EBS snapshot to copy
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
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