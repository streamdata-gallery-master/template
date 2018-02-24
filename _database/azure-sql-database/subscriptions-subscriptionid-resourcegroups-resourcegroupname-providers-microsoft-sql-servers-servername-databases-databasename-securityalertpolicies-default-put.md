---
swagger: "2.0"
info:
  title: Azure SQL Database
  description: Provides create, read, update and delete functionality for Azure SQL
    Database resources including servers, databases, elastic pools, recommendations,
    operations, and usage metrics.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/securityAlertPolicies/default
  : put:
      summary: Databases Create Or Update Threat Detection Policy
      description: Creates or updates a database's threat detection policy
      operationId: Databases_CreateOrUpdateThreatDetectionPolicy
      parameters:
      - in: path
        name: databaseName
        description: The name of the database for which database Threat Detection
          policy is defined
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The database Threat Detection policy
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - databases threat detection policy
definitions:
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
  TrackedResource:
    properties:
      tags:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
  RestorePointProperties:
    properties:
      restorePointType:
        description: This is a default description.
        type: get
      restorePointCreationDate:
        description: This is a default description.
        type: get
      earliestRestoreDate:
        description: This is a default description.
        type: get
  RestorePoint:
    properties: []
  RestorePointListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  MaxSizeCapability:
    properties:
      limit:
        description: This is a default description.
        type: get
      unit:
        description: This is a default description.
        type: get
  ServiceObjectiveCapability:
    properties:
      name:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      supportedMaxSizes:
        description: This is a default description.
        type: get
  PerformanceLevel:
    properties:
      unit:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  EditionCapability:
    properties:
      name:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      supportedServiceLevelObjectives:
        description: This is a default description.
        type: get
  ServerVersionCapability:
    properties:
      name:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      supportedEditions:
        description: This is a default description.
        type: get
      supportedElasticPoolEditions:
        description: This is a default description.
        type: get
  LocationCapabilities:
    properties:
      name:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      supportedServerVersions:
        description: This is a default description.
        type: get
  ElasticPoolEditionCapability:
    properties:
      name:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      supportedElasticPoolDtus:
        description: This is a default description.
        type: get
  ElasticPoolDtuCapability:
    properties:
      limit:
        description: This is a default description.
        type: get
      maxDatabaseCount:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      supportedMaxSizes:
        description: This is a default description.
        type: get
      supportedPerDatabaseMaxSizes:
        description: This is a default description.
        type: get
      supportedPerDatabaseMaxDtus:
        description: This is a default description.
        type: get
  ElasticPoolPerDatabaseMaxDtuCapability:
    properties:
      limit:
        description: This is a default description.
        type: get
      supportedPerDatabaseMinDtus:
        description: This is a default description.
        type: get
  ElasticPoolPerDatabaseMinDtuCapability:
    properties:
      limit:
        description: This is a default description.
        type: get
  DatabaseSecurityAlertPolicy:
    properties:
      location:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
  DatabaseSecurityAlertPolicyProperties:
    properties:
      state:
        description: This is a default description.
        type: put
      disabledAlerts:
        description: This is a default description.
        type: put
      emailAddresses:
        description: This is a default description.
        type: put
      emailAccountAdmins:
        description: This is a default description.
        type: put
      storageEndpoint:
        description: This is a default description.
        type: put
      storageAccountAccessKey:
        description: This is a default description.
        type: put
      retentionDays:
        description: This is a default description.
        type: put
      useServerDefault:
        description: This is a default description.
        type: put
  SubResource:
    properties:
      name:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
  FirewallRuleProperties:
    properties:
      startIpAddress:
        description: This is a default description.
        type: get
      endIpAddress:
        description: This is a default description.
        type: get
  FirewallRule:
    properties:
      kind:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  FirewallRuleListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  ImportExtensionProperties:
    properties:
      operationMode:
        description: This is a default description.
        type: post
  ImportExtensionRequest:
    properties:
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  ImportExportResponse:
    properties: []
  ImportExportResponseProperties:
    properties:
      requestType:
        description: This is a default description.
        type: post
      requestId:
        description: This is a default description.
        type: post
      serverName:
        description: This is a default description.
        type: post
      databaseName:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      lastModifiedTime:
        description: This is a default description.
        type: post
      queuedTime:
        description: This is a default description.
        type: post
      blobUri:
        description: This is a default description.
        type: post
      errorMessage:
        description: This is a default description.
        type: post
  ImportRequest:
    properties:
      databaseName:
        description: This is a default description.
        type: post
      edition:
        description: This is a default description.
        type: post
      serviceObjectiveName:
        description: This is a default description.
        type: post
      maxSizeBytes:
        description: This is a default description.
        type: post
  ExportRequest:
    properties:
      storageKeyType:
        description: This is a default description.
        type: post
      storageKey:
        description: This is a default description.
        type: post
      storageUri:
        description: This is a default description.
        type: post
      administratorLogin:
        description: This is a default description.
        type: post
      administratorLoginPassword:
        description: This is a default description.
        type: post
      authenticationType:
        description: This is a default description.
        type: post
  OperationListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  Operation:
    properties:
      name:
        description: This is a default description.
        type: get
  ReplicationLinkProperties:
    properties:
      isTerminationAllowed:
        description: This is a default description.
        type: get
      replicationMode:
        description: This is a default description.
        type: get
      partnerServer:
        description: This is a default description.
        type: get
      partnerDatabase:
        description: This is a default description.
        type: get
      partnerLocation:
        description: This is a default description.
        type: get
      role:
        description: This is a default description.
        type: get
      partnerRole:
        description: This is a default description.
        type: get
      startTime:
        description: This is a default description.
        type: get
      percentComplete:
        description: This is a default description.
        type: get
      replicationState:
        description: This is a default description.
        type: get
  ReplicationLink:
    properties:
      location:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
  ReplicationLinkListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  ServerProperties:
    properties:
      fullyQualifiedDomainName:
        description: This is a default description.
        type: get
      version:
        description: This is a default description.
        type: get
      administratorLogin:
        description: This is a default description.
        type: get
      administratorLoginPassword:
        description: This is a default description.
        type: get
      externalAdministratorSid:
        description: This is a default description.
        type: get
      externalAdministratorLogin:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
  Server:
    properties:
      kind:
        description: This is a default description.
        type: get
  ServerListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  ServerMetric:
    properties:
      name:
        description: This is a default description.
        type: get
      resourceName:
        description: This is a default description.
        type: get
      displayName:
        description: This is a default description.
        type: get
      currentValue:
        description: This is a default description.
        type: get
      limit:
        description: This is a default description.
        type: get
      unit:
        description: This is a default description.
        type: get
      nextResetTime:
        description: This is a default description.
        type: get
  ServerMetricListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  RecommendedElasticPoolMetric:
    properties:
      dateTime:
        description: This is a default description.
        type: get
      dtu:
        description: This is a default description.
        type: get
      sizeGB:
        description: This is a default description.
        type: get
  RecommendedElasticPoolProperties:
    properties:
      databaseEdition:
        description: This is a default description.
        type: get
      dtu:
        description: This is a default description.
        type: get
      databaseDtuMin:
        description: This is a default description.
        type: get
      databaseDtuMax:
        description: This is a default description.
        type: get
      storageMB:
        description: This is a default description.
        type: get
      observationPeriodStart:
        description: This is a default description.
        type: get
      observationPeriodEnd:
        description: This is a default description.
        type: get
      maxObservedDtu:
        description: This is a default description.
        type: get
      maxObservedStorageMB:
        description: This is a default description.
        type: get
      databases:
        description: This is a default description.
        type: get
  RecommendedElasticPool:
    properties: []
  RecommendedElasticPoolListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  RecommendedElasticPoolListMetricsResult:
    properties:
      value:
        description: This is a default description.
        type: get
  ElasticPoolProperties:
    properties:
      creationDate:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      edition:
        description: This is a default description.
        type: get
      dtu:
        description: This is a default description.
        type: get
      databaseDtuMax:
        description: This is a default description.
        type: get
      databaseDtuMin:
        description: This is a default description.
        type: get
      storageMB:
        description: This is a default description.
        type: get
  ElasticPool:
    properties:
      kind:
        description: This is a default description.
        type: get
  ElasticPoolListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  ElasticPoolActivityProperties:
    properties:
      endTime:
        description: This is a default description.
        type: get
      errorCode:
        description: This is a default description.
        type: get
      errorMessage:
        description: This is a default description.
        type: get
      errorSeverity:
        description: This is a default description.
        type: get
      operation:
        description: This is a default description.
        type: get
      operationId:
        description: This is a default description.
        type: get
      percentComplete:
        description: This is a default description.
        type: get
      requestedDatabaseDtuMax:
        description: This is a default description.
        type: get
      requestedDatabaseDtuMin:
        description: This is a default description.
        type: get
      requestedDtu:
        description: This is a default description.
        type: get
  ElasticPoolActivity:
    properties:
      location:
        description: This is a default description.
        type: get
  ElasticPoolActivityListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  ElasticPoolDatabaseActivityProperties:
    properties:
      databaseName:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
      errorCode:
        description: This is a default description.
        type: get
      errorMessage:
        description: This is a default description.
        type: get
      errorSeverity:
        description: This is a default description.
        type: get
      operation:
        description: This is a default description.
        type: get
      operationId:
        description: This is a default description.
        type: get
      percentComplete:
        description: This is a default description.
        type: get
      requestedElasticPoolName:
        description: This is a default description.
        type: get
      currentElasticPoolName:
        description: This is a default description.
        type: get
  ElasticPoolDatabaseActivity:
    properties:
      location:
        description: This is a default description.
        type: get
  ElasticPoolDatabaseActivityListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  RecommendedIndexProperties:
    properties:
      action:
        description: This is a default description.
        type: get
      state:
        description: This is a default description.
        type: get
      created:
        description: This is a default description.
        type: get
      lastModified:
        description: This is a default description.
        type: get
      indexType:
        description: This is a default description.
        type: get
      schema:
        description: This is a default description.
        type: get
      table:
        description: This is a default description.
        type: get
      columns:
        description: This is a default description.
        type: get
      includedColumns:
        description: This is a default description.
        type: get
      indexScript:
        description: This is a default description.
        type: get
  RecommendedIndex:
    properties: []
  TransparentDataEncryptionProperties:
    properties:
      status:
        description: This is a default description.
        type: get
  TransparentDataEncryption:
    properties: []
  DatabaseProperties:
    properties:
      collation:
        description: This is a default description.
        type: get
      creationDate:
        description: This is a default description.
        type: get
      containmentState:
        description: This is a default description.
        type: get
      currentServiceObjectiveId:
        description: This is a default description.
        type: get
      databaseId:
        description: This is a default description.
        type: get
      earliestRestoreDate:
        description: This is a default description.
        type: get
      createMode:
        description: This is a default description.
        type: get
      sourceDatabaseId:
        description: This is a default description.
        type: get
      sourceDatabaseDeletionDate:
        description: This is a default description.
        type: get
      restorePointInTime:
        description: This is a default description.
        type: get
  Database:
    properties:
      kind:
        description: This is a default description.
        type: get
  DatabaseListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  ServiceTierAdvisorProperties:
    properties:
      observationPeriodStart:
        description: This is a default description.
        type: get
      observationPeriodEnd:
        description: This is a default description.
        type: get
      activeTimeRatio:
        description: This is a default description.
        type: get
      minDtu:
        description: This is a default description.
        type: get
      avgDtu:
        description: This is a default description.
        type: get
      maxDtu:
        description: This is a default description.
        type: get
      maxSizeInGB:
        description: This is a default description.
        type: get
      serviceLevelObjectiveUsageMetrics:
        description: This is a default description.
        type: get
      currentServiceLevelObjective:
        description: This is a default description.
        type: get
      currentServiceLevelObjectiveId:
        description: This is a default description.
        type: get
  ServiceTierAdvisor:
    properties: []
  SloUsageMetric:
    properties:
      serviceLevelObjective:
        description: This is a default description.
        type: get
      serviceLevelObjectiveId:
        description: This is a default description.
        type: get
      inRangeTimeRatio:
        description: This is a default description.
        type: get
  OperationImpact:
    properties:
      name:
        description: This is a default description.
        type: get
      unit:
        description: This is a default description.
        type: get
      changeValueAbsolute:
        description: This is a default description.
        type: get
      changeValueRelative:
        description: This is a default description.
        type: get
  DatabaseMetric:
    properties:
      resourceName:
        description: This is a default description.
        type: get
      displayName:
        description: This is a default description.
        type: get
      currentValue:
        description: This is a default description.
        type: get
      limit:
        description: This is a default description.
        type: get
      unit:
        description: This is a default description.
        type: get
      nextResetTime:
        description: This is a default description.
        type: get
  DatabaseMetricListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  ServiceTierAdvisorListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  ServiceObjectiveProperties:
    properties:
      serviceObjectiveName:
        description: This is a default description.
        type: get
      isDefault:
        description: This is a default description.
        type: get
      isSystem:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      enabled:
        description: This is a default description.
        type: get
  ServiceObjective:
    properties: []
  ServiceObjectiveListResult:
    properties:
      value:
        description: This is a default description.
        type: get
  TransparentDataEncryptionActivityProperties:
    properties:
      status:
        description: This is a default description.
        type: get
      percentComplete:
        description: This is a default description.
        type: get
  TransparentDataEncryptionActivity:
    properties: []
  TransparentDataEncryptionActivityListResult:
    properties:
      value:
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