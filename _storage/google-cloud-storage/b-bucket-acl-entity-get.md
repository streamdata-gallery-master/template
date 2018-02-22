---
swagger: "2.0"
info:
  title: Cloud Storage
  description: Stores and retrieves potentially large, immutable data objects.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /storage/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /b/{bucket}/acl/{entity}:
    get:
      summary: Get Bucket ACL
      description: Returns the ACL entry for the specified entity on the specified
        bucket
      operationId: storage.bucketAccessControls.get
      parameters:
      - in: path
        name: bucket
        description: Name of a bucket
      - in: path
        name: entity
        description: The entity holding the permission
      responses:
        200:
          description: OK
      tags:
      - bucket acl
definitions:
  Bucket:
    properties:
      acl:
        description: This is a default description.
        type: post
      cors:
        description: This is a default description.
        type: post
      defaultObjectAcl:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      lifecycle:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      logging:
        description: This is a default description.
        type: post
      metageneration:
        description: This is a default description.
        type: post
  BucketAccessControl:
    properties:
      bucket:
        description: This is a default description.
        type: post
      domain:
        description: This is a default description.
        type: post
      email:
        description: This is a default description.
        type: post
      entity:
        description: This is a default description.
        type: post
      entityId:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      projectTeam:
        description: This is a default description.
        type: post
      role:
        description: This is a default description.
        type: post
  BucketAccessControls:
    properties:
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  Buckets:
    properties:
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  Channel:
    properties:
      address:
        description: This is a default description.
        type: post
      expiration:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      params:
        description: This is a default description.
        type: post
      payload:
        description: This is a default description.
        type: post
      resourceId:
        description: This is a default description.
        type: post
      resourceUri:
        description: This is a default description.
        type: post
      token:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  ComposeRequest:
    properties:
      kind:
        description: This is a default description.
        type: post
      sourceObjects:
        description: This is a default description.
        type: post
  Object:
    properties:
      acl:
        description: This is a default description.
        type: post
      bucket:
        description: This is a default description.
        type: post
      cacheControl:
        description: This is a default description.
        type: post
      componentCount:
        description: This is a default description.
        type: post
      contentDisposition:
        description: This is a default description.
        type: post
      contentEncoding:
        description: This is a default description.
        type: post
      contentLanguage:
        description: This is a default description.
        type: post
      contentType:
        description: This is a default description.
        type: post
      crc32c:
        description: This is a default description.
        type: post
      customerEncryption:
        description: This is a default description.
        type: post
  ObjectAccessControl:
    properties:
      bucket:
        description: This is a default description.
        type: post
      domain:
        description: This is a default description.
        type: post
      email:
        description: This is a default description.
        type: post
      entity:
        description: This is a default description.
        type: post
      entityId:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      generation:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      object:
        description: This is a default description.
        type: post
  ObjectAccessControls:
    properties:
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  Objects:
    properties:
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
      prefixes:
        description: This is a default description.
        type: post
  Policy:
    properties:
      bindings:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      resourceId:
        description: This is a default description.
        type: post
  RewriteResponse:
    properties:
      done:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      objectSize:
        description: This is a default description.
        type: post
      rewriteToken:
        description: This is a default description.
        type: post
      totalBytesRewritten:
        description: This is a default description.
        type: post
  TestIamPermissionsResponse:
    properties:
      kind:
        description: This is a default description.
        type: post
      permissions:
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