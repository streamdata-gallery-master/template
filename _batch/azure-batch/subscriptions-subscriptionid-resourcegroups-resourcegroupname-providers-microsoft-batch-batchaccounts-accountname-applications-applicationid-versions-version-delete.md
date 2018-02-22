---
swagger: "2.0"
info:
  title: BatchManagement
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Batch/batchAccounts/{accountName}/applications/{applicationId}/versions/{version}
  : delete:
      summary: Application Package Delete
      description: Deletes an application package record and its associated binary
        file
      operationId: ApplicationPackage_Delete
      parameters:
      - in: path
        name: accountName
        description: The name of the Batch account
      - in: path
        name: applicationId
        description: The ID of the application
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group that contains the Batch account
      - in: path
        name: version
        description: The version of the application to delete
      responses:
        200:
          description: OK
      tags:
      - application package
definitions:
  AutoStorageBaseProperties:
    properties:
      storageAccountId:
        description: This is a default description.
        type: get
  BatchAccountBaseProperties:
    properties: []
  BatchAccountUpdateBaseProperties:
    properties: []
  BatchAccountCreateParameters:
    properties:
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  KeyVaultReference:
    properties:
      id:
        description: This is a default description.
        type: get
      url:
        description: This is a default description.
        type: get
  AutoStorageProperties:
    properties:
      storageAccountId:
        description: This is a default description.
        type: get
      lastKeySync:
        description: This is a default description.
        type: get
  BatchAccountProperties:
    properties:
      accountEndpoint:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
      coreQuota:
        description: This is a default description.
        type: get
      poolQuota:
        description: This is a default description.
        type: get
      activeJobAndJobScheduleQuota:
        description: This is a default description.
        type: get
  BatchAccount:
    properties: []
  BatchAccountUpdateParameters:
    properties:
      tags:
        description: This is a default description.
        type: get
  BatchAccountListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  BatchAccountRegenerateKeyParameters:
    properties:
      keyName:
        description: This is a default description.
        type: get
  BatchAccountKeys:
    properties:
      primary:
        description: This is a default description.
        type: get
      secondary:
        description: This is a default description.
        type: get
  ActivateApplicationPackageParameters:
    properties:
      format:
        description: This is a default description.
        type: get
  AddApplicationParameters:
    properties:
      allowUpdates:
        description: This is a default description.
        type: get
      displayName:
        description: This is a default description.
        type: get
  Application:
    properties:
      id:
        description: This is a default description.
        type: get
      displayName:
        description: This is a default description.
        type: get
      packages:
        description: This is a default description.
        type: get
      allowUpdates:
        description: This is a default description.
        type: get
      defaultVersion:
        description: This is a default description.
        type: get
  ApplicationPackage:
    properties:
      id:
        description: This is a default description.
        type: get
      version:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      format:
        description: This is a default description.
        type: get
      storageUrl:
        description: This is a default description.
        type: get
      storageUrlExpiry:
        description: This is a default description.
        type: get
      lastActivationTime:
        description: This is a default description.
        type: get
  ListApplicationsResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  UpdateApplicationParameters:
    properties:
      allowUpdates:
        description: This is a default description.
        type: get
      defaultVersion:
        description: This is a default description.
        type: get
      displayName:
        description: This is a default description.
        type: get
  BatchLocationQuota:
    properties:
      accountQuota:
        description: This is a default description.
        type: get
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  CloudError:
    properties:
      code:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      target:
        description: This is a default description.
        type: get
      details:
        description: This is a default description.
        type: get
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