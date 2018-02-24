---
swagger: "2.0"
info:
  title: KeyVaultManagementClient
  description: The Azure management API provides a RESTful set of web services that
    interact with Azure Key Vault.
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
  /subscriptions/{subscriptionId}/resources:
    get:
      summary: Vaults List
      description: The List operation gets information about the vaults associated
        with the subscription
      operationId: Vaults_List
      parameters:
      - in: query
        name: $filter
        description: The filter to apply on the operation
      - in: query
        name: $top
        description: Maximum number of results to return
      - in: query
        name: api-version
        description: Azure Resource Manager Api Version
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - vaults
definitions:
  Sku:
    properties:
      family:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
  AccessPolicyEntry:
    properties:
      tenantId:
        description: This is a default description.
        type: get
      objectId:
        description: This is a default description.
        type: get
      applicationId:
        description: This is a default description.
        type: get
  Permissions:
    properties:
      keys:
        description: This is a default description.
        type: get
      secrets:
        description: This is a default description.
        type: get
      certificates:
        description: This is a default description.
        type: get
  VaultProperties:
    properties:
      vaultUri:
        description: This is a default description.
        type: get
      tenantId:
        description: This is a default description.
        type: get
      accessPolicies:
        description: This is a default description.
        type: get
      enabledForDeployment:
        description: This is a default description.
        type: get
      enabledForDiskEncryption:
        description: This is a default description.
        type: get
      enabledForTemplateDeployment:
        description: This is a default description.
        type: get
  VaultCreateOrUpdateParameters:
    properties:
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  Vault:
    properties: []
  VaultListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ResourceListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
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