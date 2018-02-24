---
swagger: "2.0"
info:
  title: RecoveryServicesClient
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
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}:
    delete:
      summary: Vaults Delete
      description: Deletes a vault
      operationId: Vaults_Delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - vaults
definitions:
  BackupStorageConfigProperties:
    properties:
      storageModelType:
        description: This is a default description.
        type: patch
      storageType:
        description: This is a default description.
        type: patch
      storageTypeState:
        description: This is a default description.
        type: patch
  BackupStorageConfig:
    properties: []
  BackupVaultConfigProperties:
    properties:
      storageType:
        description: This is a default description.
        type: patch
      storageTypeState:
        description: This is a default description.
        type: patch
      enhancedSecurityState:
        description: This is a default description.
        type: patch
  BackupVaultConfig:
    properties: []
  CertificateRequest:
    properties: []
  RawCertificateData:
    properties:
      authType:
        description: This is a default description.
        type: delete
      certificate:
        description: This is a default description.
        type: delete
  ResourceCertificateAndAadDetails:
    properties:
      aadAuthority:
        description: This is a default description.
        type: delete
      aadTenantId:
        description: This is a default description.
        type: delete
      servicePrincipalClientId:
        description: This is a default description.
        type: delete
      servicePrincipalObjectId:
        description: This is a default description.
        type: delete
      azureManagementEndpointAudience:
        description: This is a default description.
        type: delete
  ResourceCertificateAndAcsDetails:
    properties:
      globalAcsNamespace:
        description: This is a default description.
        type: delete
      globalAcsHostName:
        description: This is a default description.
        type: delete
      globalAcsRPRealm:
        description: This is a default description.
        type: delete
  ResourceCertificateDetails:
    properties:
      authType:
        description: This is a default description.
        type: delete
      certificate:
        description: This is a default description.
        type: delete
      friendlyName:
        description: This is a default description.
        type: delete
      issuer:
        description: This is a default description.
        type: delete
      resourceId:
        description: This is a default description.
        type: delete
      subject:
        description: This is a default description.
        type: delete
      thumbprint:
        description: This is a default description.
        type: delete
      validFrom:
        description: This is a default description.
        type: delete
      validTo:
        description: This is a default description.
        type: delete
  VaultCertificateResponse:
    properties:
      name:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      id:
        description: This is a default description.
        type: delete
  JobsSummary:
    properties:
      failedJobs:
        description: This is a default description.
        type: get
      suspendedJobs:
        description: This is a default description.
        type: get
      inProgressJobs:
        description: This is a default description.
        type: get
  MonitoringSummary:
    properties:
      unHealthyVmCount:
        description: This is a default description.
        type: get
      unHealthyProviderCount:
        description: This is a default description.
        type: get
      eventsCount:
        description: This is a default description.
        type: get
      deprecatedProviderCount:
        description: This is a default description.
        type: get
      supportedProviderCount:
        description: This is a default description.
        type: get
      unsupportedProviderCount:
        description: This is a default description.
        type: get
  ReplicationUsage:
    properties:
      protectedItemCount:
        description: This is a default description.
        type: get
      recoveryPlanCount:
        description: This is a default description.
        type: get
      registeredServersCount:
        description: This is a default description.
        type: get
      recoveryServicesProviderAuthType:
        description: This is a default description.
        type: get
  ReplicationUsageList:
    properties:
      value:
        description: This is a default description.
        type: get
  ClientDiscoveryDisplay:
    properties:
      Provider:
        description: This is a default description.
        type: patch
      Resource:
        description: This is a default description.
        type: patch
      Operation:
        description: This is a default description.
        type: patch
      Description:
        description: This is a default description.
        type: patch
  ClientDiscoveryForLogSpecification:
    properties:
      name:
        description: This is a default description.
        type: patch
      displayName:
        description: This is a default description.
        type: patch
      blobDuration:
        description: This is a default description.
        type: patch
  ClientDiscoveryForServiceSpecification:
    properties:
      logSpecifications:
        description: This is a default description.
        type: patch
  ClientDiscoveryProperties:
    properties: []
  ClientDiscoveryResponse:
    properties:
      Value:
        description: This is a default description.
        type: patch
      NextLink:
        description: This is a default description.
        type: patch
  ClientDiscoveryValueForSingleApi:
    properties:
      Name:
        description: This is a default description.
        type: patch
      Origin:
        description: This is a default description.
        type: patch
  Resource:
    properties:
      id:
        description: This is a default description.
        type: patch
      name:
        description: This is a default description.
        type: patch
      type:
        description: This is a default description.
        type: patch
      eTag:
        description: This is a default description.
        type: patch
  Sku:
    properties:
      name:
        description: This is a default description.
        type: patch
  TrackedResource:
    properties:
      location:
        description: This is a default description.
        type: patch
      tags:
        description: This is a default description.
        type: patch
  UpgradeDetails:
    properties:
      operationId:
        description: This is a default description.
        type: patch
      startTimeUtc:
        description: This is a default description.
        type: patch
      lastUpdatedTimeUtc:
        description: This is a default description.
        type: patch
      endTimeUtc:
        description: This is a default description.
        type: patch
      status:
        description: This is a default description.
        type: patch
      message:
        description: This is a default description.
        type: patch
      triggerType:
        description: This is a default description.
        type: patch
      upgradedResourceId:
        description: This is a default description.
        type: patch
      previousResourceId:
        description: This is a default description.
        type: patch
  Vault:
    properties: []
  VaultExtendedInfo:
    properties:
      integrityKey:
        description: This is a default description.
        type: patch
      encryptionKey:
        description: This is a default description.
        type: patch
      encryptionKeyThumbprint:
        description: This is a default description.
        type: patch
      algorithm:
        description: This is a default description.
        type: patch
  VaultExtendedInfoResource:
    properties: []
  VaultList:
    properties:
      value:
        description: This is a default description.
        type: patch
      nextLink:
        description: This is a default description.
        type: patch
  VaultProperties:
    properties:
      provisioningState:
        description: This is a default description.
        type: patch
  VaultUsage:
    properties:
      unit:
        description: This is a default description.
        type: get
      quotaPeriod:
        description: This is a default description.
        type: get
      nextResetTime:
        description: This is a default description.
        type: get
      currentValue:
        description: This is a default description.
        type: get
      limit:
        description: This is a default description.
        type: get
  VaultUsageList:
    properties:
      value:
        description: This is a default description.
        type: get
  NameInfo:
    properties:
      value:
        description: This is a default description.
        type: get
      localizedValue:
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