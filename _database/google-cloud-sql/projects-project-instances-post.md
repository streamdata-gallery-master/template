---
swagger: "2.0"
info:
  title: Cloud SQL Administration
  description: Creates and configures Cloud SQL instances, which provide fully-managed
    MySQL databases.
  contact:
    name: Google
    url: https://google.com
  version: v1beta4
host: www.googleapis.com
basePath: /sql/v1beta4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{project}/instances:
    post:
      summary: ""
      description: Creates a new Cloud SQL instance
      operationId: sql.instances.insert
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID of the project to which the newly created Cloud SQL
          instances should belong
      responses:
        200:
          description: OK
      tags:
      - ""
definitions:
  AclEntry:
    properties:
      expirationTime:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  BackupConfiguration:
    properties:
      binaryLogEnabled:
        description: This is a default description.
        type: parameters
      enabled:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      startTime:
        description: This is a default description.
        type: parameters
  BackupRun:
    properties:
      description:
        description: This is a default description.
        type: parameters
      endTime:
        description: This is a default description.
        type: parameters
      enqueuedTime:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      instance:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      startTime:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  BackupRunsListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  BinLogCoordinates:
    properties:
      binLogFileName:
        description: This is a default description.
        type: parameters
      binLogPosition:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  CloneContext:
    properties:
      destinationInstanceName:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Database:
    properties:
      charset:
        description: This is a default description.
        type: parameters
      collation:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      instance:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      project:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
  DatabaseFlags:
    properties:
      name:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  DatabaseInstance:
    properties:
      backendType:
        description: This is a default description.
        type: parameters
      connectionName:
        description: This is a default description.
        type: parameters
      currentDiskSize:
        description: This is a default description.
        type: parameters
      databaseVersion:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      failoverReplica:
        description: This is a default description.
        type: parameters
      instanceType:
        description: This is a default description.
        type: parameters
      ipAddresses:
        description: This is a default description.
        type: parameters
      ipv6Address:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  DatabasesListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ExportContext:
    properties:
      csvExportOptions:
        description: This is a default description.
        type: parameters
      databases:
        description: This is a default description.
        type: parameters
      fileType:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      sqlExportOptions:
        description: This is a default description.
        type: parameters
      uri:
        description: This is a default description.
        type: parameters
  FailoverContext:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      settingsVersion:
        description: This is a default description.
        type: parameters
  Flag:
    properties:
      allowedStringValues:
        description: This is a default description.
        type: parameters
      appliesTo:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      maxValue:
        description: This is a default description.
        type: parameters
      minValue:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      requiresRestart:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  FlagsListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ImportContext:
    properties:
      csvImportOptions:
        description: This is a default description.
        type: parameters
      database:
        description: This is a default description.
        type: parameters
      fileType:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      uri:
        description: This is a default description.
        type: parameters
  InstancesCloneRequest:
    properties: []
  InstancesExportRequest:
    properties: []
  InstancesFailoverRequest:
    properties: []
  InstancesImportRequest:
    properties: []
  InstancesListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  InstancesRestoreBackupRequest:
    properties: []
  InstancesTruncateLogRequest:
    properties: []
  IpConfiguration:
    properties:
      authorizedNetworks:
        description: This is a default description.
        type: parameters
      ipv4Enabled:
        description: This is a default description.
        type: parameters
      requireSsl:
        description: This is a default description.
        type: parameters
  IpMapping:
    properties:
      ipAddress:
        description: This is a default description.
        type: parameters
      timeToRetire:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  Labels:
    properties:
      key:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  LocationPreference:
    properties:
      followGaeApplication:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      zone:
        description: This is a default description.
        type: parameters
  MaintenanceWindow:
    properties:
      day:
        description: This is a default description.
        type: parameters
      hour:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      updateTrack:
        description: This is a default description.
        type: parameters
  MySqlReplicaConfiguration:
    properties:
      caCertificate:
        description: This is a default description.
        type: parameters
      clientCertificate:
        description: This is a default description.
        type: parameters
      clientKey:
        description: This is a default description.
        type: parameters
      connectRetryInterval:
        description: This is a default description.
        type: parameters
      dumpFilePath:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      masterHeartbeatPeriod:
        description: This is a default description.
        type: parameters
      password:
        description: This is a default description.
        type: parameters
      sslCipher:
        description: This is a default description.
        type: parameters
      username:
        description: This is a default description.
        type: parameters
  OnPremisesConfiguration:
    properties:
      hostPort:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Operation:
    properties:
      endTime:
        description: This is a default description.
        type: parameters
      insertTime:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      operationType:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      startTime:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      targetId:
        description: This is a default description.
        type: parameters
      targetLink:
        description: This is a default description.
        type: parameters
  OperationError:
    properties:
      code:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      message:
        description: This is a default description.
        type: parameters
  OperationErrors:
    properties:
      errors:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  OperationsListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  ReplicaConfiguration:
    properties:
      failoverTarget:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  RestoreBackupContext:
    properties:
      backupRunId:
        description: This is a default description.
        type: parameters
      instanceId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Settings:
    properties:
      activationPolicy:
        description: This is a default description.
        type: parameters
      authorizedGaeApplications:
        description: This is a default description.
        type: parameters
      availabilityType:
        description: This is a default description.
        type: parameters
      crashSafeReplicationEnabled:
        description: This is a default description.
        type: parameters
      dataDiskSizeGb:
        description: This is a default description.
        type: parameters
      dataDiskType:
        description: This is a default description.
        type: parameters
      databaseFlags:
        description: This is a default description.
        type: parameters
      databaseReplicationEnabled:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      labels:
        description: This is a default description.
        type: parameters
  SslCert:
    properties:
      cert:
        description: This is a default description.
        type: parameters
      certSerialNumber:
        description: This is a default description.
        type: parameters
      commonName:
        description: This is a default description.
        type: parameters
      createTime:
        description: This is a default description.
        type: parameters
      expirationTime:
        description: This is a default description.
        type: parameters
      instance:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      sha1Fingerprint:
        description: This is a default description.
        type: parameters
  SslCertDetail:
    properties:
      certPrivateKey:
        description: This is a default description.
        type: parameters
  SslCertsCreateEphemeralRequest:
    properties:
      public_key:
        description: This is a default description.
        type: parameters
  SslCertsInsertRequest:
    properties:
      commonName:
        description: This is a default description.
        type: parameters
  SslCertsInsertResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
  SslCertsListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Tier:
    properties:
      DiskQuota:
        description: This is a default description.
        type: parameters
      RAM:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      region:
        description: This is a default description.
        type: parameters
      tier:
        description: This is a default description.
        type: parameters
  TiersListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  TruncateLogContext:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      logType:
        description: This is a default description.
        type: parameters
  User:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      host:
        description: This is a default description.
        type: parameters
      instance:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      password:
        description: This is a default description.
        type: parameters
      project:
        description: This is a default description.
        type: parameters
  UsersListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
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