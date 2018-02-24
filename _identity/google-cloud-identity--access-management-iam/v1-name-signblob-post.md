---
swagger: "2.0"
info:
  title: Google Identity and Access Management (IAM)
  description: Manages identity and access control for Google Cloud Platform resources,
    including the creation of service accounts, which you can use to authenticate
    to Google and make API calls.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: iam.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{name}:signBlob:
    post:
      summary: Sign Blob
      description: Signs a blob using a service account's system-managed private key
      operationId: iam.projects.serviceAccounts.signBlob
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: name
        description: |-
          The resource name of the service account in the following format:
          `projects/{PROJECT_ID}/serviceAccounts/{SERVICE_ACCOUNT_EMAIL}`
      responses:
        200:
          description: OK
      tags:
      - blob
definitions:
  AuditData:
    properties: []
  Binding:
    properties:
      members:
        description: This is a default description.
        type: post
      role:
        description: This is a default description.
        type: post
  BindingDelta:
    properties:
      action:
        description: This is a default description.
        type: post
      member:
        description: This is a default description.
        type: post
      role:
        description: This is a default description.
        type: post
  CreateServiceAccountKeyRequest:
    properties:
      keyAlgorithm:
        description: This is a default description.
        type: post
      privateKeyType:
        description: This is a default description.
        type: post
  CreateServiceAccountRequest:
    properties:
      accountId:
        description: This is a default description.
        type: post
  Empty:
    properties: []
  ListServiceAccountKeysResponse:
    properties:
      keys:
        description: This is a default description.
        type: post
  ListServiceAccountsResponse:
    properties:
      accounts:
        description: This is a default description.
        type: post
      nextPageToken:
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
      version:
        description: This is a default description.
        type: post
  PolicyDelta:
    properties:
      bindingDeltas:
        description: This is a default description.
        type: post
  QueryGrantableRolesRequest:
    properties:
      fullResourceName:
        description: This is a default description.
        type: post
  QueryGrantableRolesResponse:
    properties:
      roles:
        description: This is a default description.
        type: post
  Role:
    properties:
      description:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      title:
        description: This is a default description.
        type: post
  ServiceAccount:
    properties:
      displayName:
        description: This is a default description.
        type: post
      email:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      oauth2ClientId:
        description: This is a default description.
        type: post
      projectId:
        description: This is a default description.
        type: post
      uniqueId:
        description: This is a default description.
        type: post
  ServiceAccountKey:
    properties:
      keyAlgorithm:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      privateKeyData:
        description: This is a default description.
        type: post
      privateKeyType:
        description: This is a default description.
        type: post
      publicKeyData:
        description: This is a default description.
        type: post
      validAfterTime:
        description: This is a default description.
        type: post
      validBeforeTime:
        description: This is a default description.
        type: post
  SetIamPolicyRequest:
    properties: []
  SignBlobRequest:
    properties:
      bytesToSign:
        description: This is a default description.
        type: post
  SignBlobResponse:
    properties:
      keyId:
        description: This is a default description.
        type: post
      signature:
        description: This is a default description.
        type: post
  SignJwtRequest:
    properties:
      payload:
        description: This is a default description.
        type: post
  SignJwtResponse:
    properties:
      keyId:
        description: This is a default description.
        type: post
      signedJwt:
        description: This is a default description.
        type: post
  TestIamPermissionsRequest:
    properties:
      permissions:
        description: This is a default description.
        type: post
  TestIamPermissionsResponse:
    properties:
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