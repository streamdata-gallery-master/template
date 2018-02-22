---
swagger: "2.0"
info:
  title: ServiceFabricManagementClient
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
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ServiceFabric/clusters/{clusterName}:
    put:
      summary: Clusters Create
      description: Create cluster resource
      operationId: Clusters_Create
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Put Request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - clusters
definitions:
  ClusterVersionDetails:
    properties:
      codeVersion:
        description: This is a default description.
        type: get
      supportExpiryUtc:
        description: This is a default description.
        type: get
  ClusterCodeVersionsResult:
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
  ClusterCodeVersionsListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  CertificateDescription:
    properties:
      thumbprint:
        description: This is a default description.
        type: get
      thumbprintSecondary:
        description: This is a default description.
        type: get
      x509StoreName:
        description: This is a default description.
        type: get
  SettingsParameterDescription:
    properties:
      name:
        description: This is a default description.
        type: get
      value:
        description: This is a default description.
        type: get
  SettingsSectionDescription:
    properties:
      name:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
  EndpointRangeDescription:
    properties:
      startPort:
        description: This is a default description.
        type: get
      endPort:
        description: This is a default description.
        type: get
  NodeTypeDescription:
    properties:
      name:
        description: This is a default description.
        type: get
      placementProperties:
        description: This is a default description.
        type: get
      capacities:
        description: This is a default description.
        type: get
      clientConnectionEndpointPort:
        description: This is a default description.
        type: get
      httpGatewayEndpointPort:
        description: This is a default description.
        type: get
      durabilityLevel:
        description: This is a default description.
        type: get
      isPrimary:
        description: This is a default description.
        type: get
      vmInstanceCount:
        description: This is a default description.
        type: get
      reverseProxyEndpointPort:
        description: This is a default description.
        type: get
  ClientCertificateThumbprint:
    properties:
      isAdmin:
        description: This is a default description.
        type: get
      certificateThumbprint:
        description: This is a default description.
        type: get
  ClientCertificateCommonName:
    properties:
      isAdmin:
        description: This is a default description.
        type: get
      certificateCommonName:
        description: This is a default description.
        type: get
      certificateIssuerThumbprint:
        description: This is a default description.
        type: get
  ClusterHealthPolicy:
    properties:
      maxPercentUnhealthyNodes:
        description: This is a default description.
        type: get
      maxPercentUnhealthyApplications:
        description: This is a default description.
        type: get
  ClusterUpgradeDeltaHealthPolicy:
    properties:
      maxPercentDeltaUnhealthyNodes:
        description: This is a default description.
        type: get
      maxPercentUpgradeDomainDeltaUnhealthyNodes:
        description: This is a default description.
        type: get
      maxPercentDeltaUnhealthyApplications:
        description: This is a default description.
        type: get
  ClusterUpgradePolicy:
    properties:
      overrideUserUpgradePolicy:
        description: This is a default description.
        type: get
      forceRestart:
        description: This is a default description.
        type: get
      upgradeReplicaSetCheckTimeout:
        description: This is a default description.
        type: get
      healthCheckWaitDuration:
        description: This is a default description.
        type: get
      healthCheckStableDuration:
        description: This is a default description.
        type: get
      healthCheckRetryTimeout:
        description: This is a default description.
        type: get
      upgradeTimeout:
        description: This is a default description.
        type: get
      upgradeDomainTimeout:
        description: This is a default description.
        type: get
  DiagnosticsStorageAccountConfig:
    properties:
      storageAccountName:
        description: This is a default description.
        type: get
      protectedAccountKeyName:
        description: This is a default description.
        type: get
      blobEndpoint:
        description: This is a default description.
        type: get
      queueEndpoint:
        description: This is a default description.
        type: get
      tableEndpoint:
        description: This is a default description.
        type: get
  AzureActiveDirectory:
    properties:
      tenantId:
        description: This is a default description.
        type: get
      clusterApplication:
        description: This is a default description.
        type: get
      clientApplication:
        description: This is a default description.
        type: get
  ClusterPropertiesUpdateParameters:
    properties:
      reliabilityLevel:
        description: This is a default description.
        type: get
      upgradeMode:
        description: This is a default description.
        type: get
      clusterCodeVersion:
        description: This is a default description.
        type: get
      clientCertificateThumbprints:
        description: This is a default description.
        type: get
      clientCertificateCommonNames:
        description: This is a default description.
        type: get
      fabricSettings:
        description: This is a default description.
        type: get
      nodeTypes:
        description: This is a default description.
        type: get
  ClusterProperties:
    properties:
      availableClusterVersions:
        description: This is a default description.
        type: get
      clusterId:
        description: This is a default description.
        type: get
      clusterState:
        description: This is a default description.
        type: get
      clusterEndpoint:
        description: This is a default description.
        type: get
      clusterCodeVersion:
        description: This is a default description.
        type: get
      reliabilityLevel:
        description: This is a default description.
        type: get
      upgradeMode:
        description: This is a default description.
        type: get
      clientCertificateThumbprints:
        description: This is a default description.
        type: get
      clientCertificateCommonNames:
        description: This is a default description.
        type: get
      fabricSettings:
        description: This is a default description.
        type: get
  ClusterUpdateParameters:
    properties:
      tags:
        description: This is a default description.
        type: get
  Cluster:
    properties: []
  ClusterListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  AvailableOperationDisplay:
    properties:
      provider:
        description: This is a default description.
        type: get
      resource:
        description: This is a default description.
        type: get
      operation:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
  OperationResult:
    properties:
      name:
        description: This is a default description.
        type: get
      origin:
        description: This is a default description.
        type: get
      nextLink:
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
  ErrorModel:
    properties: []
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