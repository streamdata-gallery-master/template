---
swagger: "2.0"
info:
  title: Google Container Engine
  description: Builds and manages clusters that run container-based applications,
    powered by open source Kubernetes technology.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: container.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}/zones/{zone}/clusters/{clusterId}/nodePools/{nodePoolId}:
    get:
      summary: Get Cluster Node Pool
      description: Retrieves the node pool requested
      operationId: container.projects.zones.clusters.nodePools.get
      parameters:
      - in: path
        name: clusterId
        description: The name of the cluster
      - in: path
        name: nodePoolId
        description: The name of the node pool
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://developers
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          in which the cluster resides
      responses:
        200:
          description: OK
      tags:
      - node pool
definitions:
  AddonsConfig:
    properties: []
  AutoUpgradeOptions:
    properties:
      autoUpgradeStartTime:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
  Cluster:
    properties:
      clusterIpv4Cidr:
        description: This is a default description.
        type: parameters
      createTime:
        description: This is a default description.
        type: parameters
      currentMasterVersion:
        description: This is a default description.
        type: parameters
      currentNodeCount:
        description: This is a default description.
        type: parameters
      currentNodeVersion:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      enableKubernetesAlpha:
        description: This is a default description.
        type: parameters
      endpoint:
        description: This is a default description.
        type: parameters
      expireTime:
        description: This is a default description.
        type: parameters
      initialClusterVersion:
        description: This is a default description.
        type: parameters
  ClusterUpdate:
    properties:
      desiredImageType:
        description: This is a default description.
        type: parameters
      desiredLocations:
        description: This is a default description.
        type: parameters
      desiredMasterVersion:
        description: This is a default description.
        type: parameters
      desiredMonitoringService:
        description: This is a default description.
        type: parameters
      desiredNodePoolId:
        description: This is a default description.
        type: parameters
      desiredNodeVersion:
        description: This is a default description.
        type: parameters
  CreateClusterRequest:
    properties: []
  CreateNodePoolRequest:
    properties: []
  HorizontalPodAutoscaling:
    properties:
      disabled:
        description: This is a default description.
        type: parameters
  HttpLoadBalancing:
    properties:
      disabled:
        description: This is a default description.
        type: parameters
  ListClustersResponse:
    properties:
      clusters:
        description: This is a default description.
        type: parameters
      missingZones:
        description: This is a default description.
        type: parameters
  ListNodePoolsResponse:
    properties:
      nodePools:
        description: This is a default description.
        type: parameters
  ListOperationsResponse:
    properties:
      missingZones:
        description: This is a default description.
        type: parameters
      operations:
        description: This is a default description.
        type: parameters
  MasterAuth:
    properties:
      clientCertificate:
        description: This is a default description.
        type: parameters
      clientKey:
        description: This is a default description.
        type: parameters
      clusterCaCertificate:
        description: This is a default description.
        type: parameters
      password:
        description: This is a default description.
        type: parameters
      username:
        description: This is a default description.
        type: parameters
  NodeConfig:
    properties:
      diskSizeGb:
        description: This is a default description.
        type: parameters
      imageType:
        description: This is a default description.
        type: parameters
      labels:
        description: This is a default description.
        type: parameters
      localSsdCount:
        description: This is a default description.
        type: parameters
      machineType:
        description: This is a default description.
        type: parameters
      metadata:
        description: This is a default description.
        type: parameters
      oauthScopes:
        description: This is a default description.
        type: parameters
      preemptible:
        description: This is a default description.
        type: parameters
      serviceAccount:
        description: This is a default description.
        type: parameters
      tags:
        description: This is a default description.
        type: parameters
  NodeManagement:
    properties:
      autoUpgrade:
        description: This is a default description.
        type: parameters
  NodePool:
    properties:
      initialNodeCount:
        description: This is a default description.
        type: parameters
      instanceGroupUrls:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      selfLink:
        description: This is a default description.
        type: parameters
      status:
        description: This is a default description.
        type: parameters
      statusMessage:
        description: This is a default description.
        type: parameters
      version:
        description: This is a default description.
        type: parameters
  NodePoolAutoscaling:
    properties:
      enabled:
        description: This is a default description.
        type: parameters
      maxNodeCount:
        description: This is a default description.
        type: parameters
      minNodeCount:
        description: This is a default description.
        type: parameters
  Operation:
    properties:
      detail:
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
      status:
        description: This is a default description.
        type: parameters
      statusMessage:
        description: This is a default description.
        type: parameters
      targetLink:
        description: This is a default description.
        type: parameters
      zone:
        description: This is a default description.
        type: parameters
  ServerConfig:
    properties:
      defaultClusterVersion:
        description: This is a default description.
        type: parameters
      defaultImageType:
        description: This is a default description.
        type: parameters
      validImageTypes:
        description: This is a default description.
        type: parameters
      validMasterVersions:
        description: This is a default description.
        type: parameters
      validNodeVersions:
        description: This is a default description.
        type: parameters
  SetNodePoolManagementRequest:
    properties: []
  UpdateClusterRequest:
    properties: []
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