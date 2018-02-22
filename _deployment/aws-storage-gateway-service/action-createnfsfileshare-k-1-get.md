---
swagger: "2.0"
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateNFSFileShare&k=1:
    get:
      summary: ' Create NFS File Share '
      description: Creates a file share on an existing file gateway
      operationId: createNFSFileShare
      parameters:
      - in: query
        name: ClientToken
        description: A unique string value that you supply that is used by file gateway
          to ensure         idempotent file share creation
        type: string
      - in: query
        name: DefaultStorageClass
        description: The default storage class for objects put into an Amazon S3 bucket
          by file gateway
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the file gateway on which you
          want to create a file share
        type: string
      - in: query
        name: KMSEncrypted
        description: True to use Amazon S3 server side encryption with your own AWS
          KMS key, or false to         use a key managed by Amazon S3
        type: string
      - in: query
        name: KMSKey
        description: The KMS key used for Amazon S3 server side encryption
        type: string
      - in: query
        name: LocationARN
        description: The ARN of the backend storage used for storing file data
        type: string
      - in: query
        name: NFSFileShareDefaults
        description: File share default values
        type: string
      - in: query
        name: Role
        description: The ARN of the AWS Identity and Access Management (IAM) role
          that a file gateway         assumes when it accesses the underlying storage
        type: string
      responses:
        200:
          description: OK
      tags:
      - nfs file share
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