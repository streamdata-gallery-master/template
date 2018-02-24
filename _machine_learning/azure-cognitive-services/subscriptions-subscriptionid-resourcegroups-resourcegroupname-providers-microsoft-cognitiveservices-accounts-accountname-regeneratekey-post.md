---
swagger: "2.0"
info:
  title: CognitiveServicesManagementClient
  description: Cognitive Services Management Client
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.CognitiveServices/accounts/{accountName}/regenerateKey
  : post:
      summary: Cognitive Services Accounts Regenerate Key
      description: Regenerates the specified account key for the specified Cognitive
        Services account
      operationId: CognitiveServicesAccounts_RegenerateKey
      parameters:
      - in: path
        name: accountName
        description: The name of Cognitive Services account
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: regenerate key parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group within the user's subscription
      responses:
        200:
          description: OK
      tags:
      - cognitive service
definitions:
  CognitiveServicesAccountCreateParameters:
    properties:
      location:
        description: This is a default description.
        type: post
      tags:
        description: This is a default description.
        type: post
      properties:
        description: This is a default description.
        type: post
  CognitiveServicesAccountUpdateParameters:
    properties:
      tags:
        description: This is a default description.
        type: post
  Sku:
    properties:
      name:
        description: This is a default description.
        type: post
      tier:
        description: This is a default description.
        type: post
  CognitiveServicesAccount:
    properties:
      etag:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      tags:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  CognitiveServicesAccountListResult:
    properties:
      nextLink:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  CognitiveServicesAccountProperties:
    properties:
      provisioningState:
        description: This is a default description.
        type: post
      endpoint:
        description: This is a default description.
        type: post
      internalId:
        description: This is a default description.
        type: post
  CognitiveServicesAccountKeys:
    properties:
      key1:
        description: This is a default description.
        type: post
      key2:
        description: This is a default description.
        type: post
  RegenerateKeyParameters:
    properties:
      keyName:
        description: This is a default description.
        type: post
  CognitiveServicesAccountEnumerateSkusResult:
    properties:
      value:
        description: This is a default description.
        type: post
  CognitiveServicesResourceAndSku:
    properties:
      resourceType:
        description: This is a default description.
        type: post
  Error:
    properties: []
  ErrorBody:
    properties:
      code:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  OperationEntityListResult:
    properties:
      nextLink:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
  OperationEntity:
    properties:
      name:
        description: This is a default description.
        type: post
      origin:
        description: This is a default description.
        type: post
      properties:
        description: This is a default description.
        type: post
  OperationDisplayInfo:
    properties:
      description:
        description: This is a default description.
        type: post
      operation:
        description: This is a default description.
        type: post
      provider:
        description: This is a default description.
        type: post
      resource:
        description: This is a default description.
        type: post
  CheckSkuAvailabilityParameter:
    properties:
      skus:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  CheckSkuAvailabilityResultList:
    properties:
      value:
        description: This is a default description.
        type: post
  CheckSkuAvailabilityResult:
    properties:
      type:
        description: This is a default description.
        type: post
      skuAvailable:
        description: This is a default description.
        type: post
      reason:
        description: This is a default description.
        type: post
      message:
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