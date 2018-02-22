---
swagger: "2.0"
info:
  title: HDInsightManagementClient
  description: The HDInsight Management Client.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/roles/{roleName}/resize
  : post:
      summary: Clusters Resize
      description: Begins a resize operation on the specified HDInsight cluster
      operationId: Clusters_Resize
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters for the resize operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: roleName
        description: The constant value for the roleName
      responses:
        200:
          description: OK
      tags:
      - clusters resize
definitions:
  ApplicationGetHttpsEndpoint:
    properties:
      accessModes:
        description: This is a default description.
        type: delete
      location:
        description: This is a default description.
        type: delete
      destinationPort:
        description: This is a default description.
        type: delete
      publicPort:
        description: This is a default description.
        type: delete
  ApplicationGetEndpoint:
    properties:
      location:
        description: This is a default description.
        type: delete
      destinationPort:
        description: This is a default description.
        type: delete
      publicPort:
        description: This is a default description.
        type: delete
  ApplicationGetProperties:
    properties:
      installScriptActions:
        description: This is a default description.
        type: delete
      uninstallScriptActions:
        description: This is a default description.
        type: delete
      httpsEndpoints:
        description: This is a default description.
        type: delete
      sshEndpoints:
        description: This is a default description.
        type: delete
      provisioningState:
        description: This is a default description.
        type: delete
      applicationType:
        description: This is a default description.
        type: delete
      applicationState:
        description: This is a default description.
        type: delete
      errors:
        description: This is a default description.
        type: delete
      createdDate:
        description: This is a default description.
        type: delete
      marketplaceIdentifier:
        description: This is a default description.
        type: delete
  Application:
    properties:
      name:
        description: This is a default description.
        type: delete
      type:
        description: This is a default description.
        type: delete
      etag:
        description: This is a default description.
        type: delete
      tags:
        description: This is a default description.
        type: delete
  ApplicationListResult:
    properties:
      value:
        description: This is a default description.
        type: delete
      nextLink:
        description: This is a default description.
        type: delete
  versionSpec:
    properties:
      friendlyName:
        description: This is a default description.
        type: get
      displayName:
        description: This is a default description.
        type: get
      isDefault:
        description: This is a default description.
        type: get
      componentVersions:
        description: This is a default description.
        type: get
  versionsCapability:
    properties:
      available:
        description: This is a default description.
        type: get
  regionsCapability:
    properties:
      available:
        description: This is a default description.
        type: get
  vmSizesCapability:
    properties:
      available:
        description: This is a default description.
        type: get
  vmSizeCompatibilityFilter:
    properties:
      FilterMode:
        description: This is a default description.
        type: get
      Regions:
        description: This is a default description.
        type: get
      ClusterFlavors:
        description: This is a default description.
        type: get
      NodeTypes:
        description: This is a default description.
        type: get
      ClusterVersions:
        description: This is a default description.
        type: get
      vmsizes:
        description: This is a default description.
        type: get
  regionalQuotaCapability:
    properties:
      region_name:
        description: This is a default description.
        type: get
      cores_used:
        description: This is a default description.
        type: get
      cores_available:
        description: This is a default description.
        type: get
  quotaCapability:
    properties:
      regionalQuotas:
        description: This is a default description.
        type: get
  capabilitiesResult:
    properties:
      versions:
        description: This is a default description.
        type: get
      regions:
        description: This is a default description.
        type: get
      vmsizes:
        description: This is a default description.
        type: get
      vmsize_filters:
        description: This is a default description.
        type: get
      features:
        description: This is a default description.
        type: get
  HttpSettingsParameters:
    properties:
      restAuthCredential.isEnabled:
        description: This is a default description.
        type: get
      restAuthCredential.username:
        description: This is a default description.
        type: get
      restAuthCredential.password:
        description: This is a default description.
        type: get
  ClusterDefinition:
    properties:
      blueprint:
        description: This is a default description.
        type: get
      kind:
        description: This is a default description.
        type: get
      componentVersion:
        description: This is a default description.
        type: get
      configurations:
        description: This is a default description.
        type: get
  SecurityProfile:
    properties:
      directoryType:
        description: This is a default description.
        type: get
      domain:
        description: This is a default description.
        type: get
      organizationalUnitDN:
        description: This is a default description.
        type: get
      ldapsUrls:
        description: This is a default description.
        type: get
      domainUsername:
        description: This is a default description.
        type: get
      domainUserPassword:
        description: This is a default description.
        type: get
      clusterUsersGroupDNs:
        description: This is a default description.
        type: get
  HardwareProfile:
    properties:
      vmSize:
        description: This is a default description.
        type: get
  VirtualNetworkProfile:
    properties:
      id:
        description: This is a default description.
        type: get
      subnet:
        description: This is a default description.
        type: get
  Role:
    properties:
      name:
        description: This is a default description.
        type: get
      minInstanceCount:
        description: This is a default description.
        type: get
      targetInstanceCount:
        description: This is a default description.
        type: get
      scriptActions:
        description: This is a default description.
        type: get
  ComputeProfile:
    properties:
      roles:
        description: This is a default description.
        type: get
  StorageAccount:
    properties:
      name:
        description: This is a default description.
        type: get
      isDefault:
        description: This is a default description.
        type: get
      container:
        description: This is a default description.
        type: get
      key:
        description: This is a default description.
        type: get
  StorageProfile:
    properties:
      storageaccounts:
        description: This is a default description.
        type: get
  ClusterCreateProperties:
    properties:
      clusterVersion:
        description: This is a default description.
        type: get
      osType:
        description: This is a default description.
        type: get
      tier:
        description: This is a default description.
        type: get
  ClusterCreateParametersExtended:
    properties:
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  ClusterPatchParameters:
    properties:
      tags:
        description: This is a default description.
        type: get
  QuotaInfo:
    properties:
      coresUsed:
        description: This is a default description.
        type: get
  errors:
    properties:
      code:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  ConnectivityEndpoint:
    properties:
      name:
        description: This is a default description.
        type: get
      protocol:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      port:
        description: This is a default description.
        type: get
  ClusterGetProperties:
    properties:
      clusterVersion:
        description: This is a default description.
        type: get
      osType:
        description: This is a default description.
        type: get
      tier:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
      createdDate:
        description: This is a default description.
        type: get
      clusterState:
        description: This is a default description.
        type: get
      errors:
        description: This is a default description.
        type: get
      connectivityEndpoints:
        description: This is a default description.
        type: get
  Cluster:
    properties:
      etag:
        description: This is a default description.
        type: get
  RuntimeScriptAction:
    properties:
      name:
        description: This is a default description.
        type: get
      uri:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
      roles:
        description: This is a default description.
        type: get
      applicationName:
        description: This is a default description.
        type: get
  ExecuteScriptActionParameters:
    properties:
      scriptActions:
        description: This is a default description.
        type: get
      persistOnSuccess:
        description: This is a default description.
        type: get
  ClusterListPersistedScriptActionsResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ScriptActionExecutionSummary:
    properties:
      status:
        description: This is a default description.
        type: get
      instanceCount:
        description: This is a default description.
        type: get
  RuntimeScriptActionDetail:
    properties:
      scriptExecutionId:
        description: This is a default description.
        type: get
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
      status:
        description: This is a default description.
        type: get
      operation:
        description: This is a default description.
        type: get
      executionSummary:
        description: This is a default description.
        type: get
      debugInformation:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      uri:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
  ClusterListRuntimeScriptActionDetailResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ClusterListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ClusterResizeParameters:
    properties:
      targetInstanceCount:
        description: This is a default description.
        type: get
  OperationResource:
    properties:
      status:
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
  SubResource:
    properties:
      id:
        description: This is a default description.
        type: get
  Operation:
    properties:
      name:
        description: This is a default description.
        type: get
  OperationListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  RdpSettings:
    properties:
      username:
        description: This is a default description.
        type: get
      password:
        description: This is a default description.
        type: get
      expiryDate:
        description: This is a default description.
        type: get
  WindowsOperatingSystemProfile:
    properties: []
  SshPublicKey:
    properties:
      certificateData:
        description: This is a default description.
        type: get
  SshProfile:
    properties:
      publicKeys:
        description: This is a default description.
        type: get
  LinuxOperatingSystemProfile:
    properties:
      username:
        description: This is a default description.
        type: get
      password:
        description: This is a default description.
        type: get
  OsProfile:
    properties: []
  RDPSettingsParameters:
    properties: []
  HttpConnectivitySettings:
    properties:
      restAuthCredential.isEnabled:
        description: This is a default description.
        type: get
      restAuthCredential.username:
        description: This is a default description.
        type: get
      restAuthCredential.password:
        description: This is a default description.
        type: get
  Extension:
    properties:
      workspaceId:
        description: This is a default description.
        type: delete
      primaryKey:
        description: This is a default description.
        type: delete
  ScriptActionExecutionHistoryList:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ScriptAction:
    properties:
      name:
        description: This is a default description.
        type: post
      uri:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
  ScriptActionPersistedGetResponseSpec:
    properties:
      name:
        description: This is a default description.
        type: post
      uri:
        description: This is a default description.
        type: post
      parameters:
        description: This is a default description.
        type: post
      roles:
        description: This is a default description.
        type: post
      applicationName:
        description: This is a default description.
        type: post
  ScriptActionsList:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
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