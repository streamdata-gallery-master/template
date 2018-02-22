---
swagger: "2.0"
info:
  title: ContainerRegistryManagementClient
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ContainerRegistry/registries/{registryName}
  : delete:
      summary: Registries Delete
      description: Deletes a container registry
      operationId: Registries_Delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - container registry
definitions:
  RegistryNameCheckRequest:
    properties:
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  RegistryNameStatus:
    properties:
      nameAvailable:
        description: This is a default description.
        type: post
      reason:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  OperationListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  OperationDefinition:
    properties:
      name:
        description: This is a default description.
        type: post
  OperationDisplayDefinition:
    properties:
      provider:
        description: This is a default description.
        type: post
      resource:
        description: This is a default description.
        type: post
      operation:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
  Registry:
    properties: []
  Sku:
    properties:
      name:
        description: This is a default description.
        type: post
      tier:
        description: This is a default description.
        type: post
  RegistryProperties:
    properties:
      loginServer:
        description: This is a default description.
        type: post
      creationDate:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      adminUserEnabled:
        description: This is a default description.
        type: post
  StorageAccountProperties:
    properties:
      name:
        description: This is a default description.
        type: post
  RegistryCreateParameters:
    properties:
      tags:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
  RegistryPropertiesCreateParameters:
    properties:
      adminUserEnabled:
        description: This is a default description.
        type: post
  StorageAccountParameters:
    properties:
      name:
        description: This is a default description.
        type: post
      accessKey:
        description: This is a default description.
        type: post
  RegistryUpdateParameters:
    properties:
      tags:
        description: This is a default description.
        type: post
  RegistryPropertiesUpdateParameters:
    properties:
      adminUserEnabled:
        description: This is a default description.
        type: post
  RegistryListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  RegistryListCredentialsResult:
    properties:
      username:
        description: This is a default description.
        type: post
      passwords:
        description: This is a default description.
        type: post
  RegistryPassword:
    properties:
      name:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  RegenerateCredentialParameters:
    properties:
      name:
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