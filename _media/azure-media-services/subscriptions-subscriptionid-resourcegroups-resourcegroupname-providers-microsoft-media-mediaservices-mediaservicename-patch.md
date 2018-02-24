---
swagger: "2.0"
info:
  title: MediaServicesManagementClient
  description: Media Services resource management APIs.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Media/mediaservices/{mediaServiceName}:
    patch:
      summary: Media Service Update
      description: Updates a Media Service
      operationId: MediaService_Update
      parameters:
      - in: body
        name: MediaService
        description: Media Service properties needed for update
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - media service
definitions:
  ApiEndpoint:
    properties:
      endpoint:
        description: This is a default description.
        type: post
      majorVersion:
        description: This is a default description.
        type: post
  ApiError:
    properties:
      code:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  CheckNameAvailabilityInput:
    properties:
      name:
        description: This is a default description.
        type: post
  CheckNameAvailabilityOutput:
    properties:
      NameAvailable:
        description: This is a default description.
        type: post
      Reason:
        description: This is a default description.
        type: post
      Message:
        description: This is a default description.
        type: post
  MediaService:
    properties: []
  MediaServiceCollection:
    properties:
      value:
        description: This is a default description.
        type: post
  MediaServiceProperties:
    properties:
      apiEndpoints:
        description: This is a default description.
        type: post
      storageAccounts:
        description: This is a default description.
        type: post
  RegenerateKeyInput:
    properties:
      keyType:
        description: This is a default description.
        type: post
  RegenerateKeyOutput:
    properties:
      key:
        description: This is a default description.
        type: post
  Resource:
    properties:
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      tags:
        description: This is a default description.
        type: post
  ServiceKeys:
    properties:
      primaryAuthEndpoint:
        description: This is a default description.
        type: post
      secondaryAuthEndpoint:
        description: This is a default description.
        type: post
      primaryKey:
        description: This is a default description.
        type: post
      secondaryKey:
        description: This is a default description.
        type: post
      scope:
        description: This is a default description.
        type: post
  StorageAccount:
    properties:
      id:
        description: This is a default description.
        type: post
      isPrimary:
        description: This is a default description.
        type: post
  SyncStorageKeysInput:
    properties:
      id:
        description: This is a default description.
        type: post
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