---
swagger: "2.0"
info:
  title: Google Cloud Dataproc
  description: Manages Hadoop-based clusters and jobs on Google Cloud Platform.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: dataproc.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}/regions/{region}/clusters/{clusterName}:
    get:
      summary: Get Cluster
      description: Gets the resource representation for a cluster in a project
      operationId: dataproc.projects.regions.clusters.get
      parameters:
      - in: path
        name: clusterName
        description: Required The cluster name
      - in: path
        name: projectId
        description: Required The ID of the Google Cloud Platform project that the
          cluster belongs to
      - in: path
        name: region
        description: Required The Cloud Dataproc region in which to handle the request
      responses:
        200:
          description: OK
      tags:
      - cluster
definitions:
  AcceleratorConfig:
    properties:
      acceleratorCount:
        description: This is a default description.
        type: post
      acceleratorTypeUri:
        description: This is a default description.
        type: post
  CancelJobRequest:
    properties: []
  Cluster:
    properties:
      clusterName:
        description: This is a default description.
        type: post
      clusterUuid:
        description: This is a default description.
        type: post
      labels:
        description: This is a default description.
        type: post
      projectId:
        description: This is a default description.
        type: post
      statusHistory:
        description: This is a default description.
        type: post
  ClusterConfig:
    properties:
      configBucket:
        description: This is a default description.
        type: post
      initializationActions:
        description: This is a default description.
        type: post
  ClusterMetrics:
    properties:
      hdfsMetrics:
        description: This is a default description.
        type: post
      yarnMetrics:
        description: This is a default description.
        type: post
  ClusterOperationMetadata:
    properties:
      clusterName:
        description: This is a default description.
        type: post
      clusterUuid:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      labels:
        description: This is a default description.
        type: post
      operationType:
        description: This is a default description.
        type: post
      statusHistory:
        description: This is a default description.
        type: post
      warnings:
        description: This is a default description.
        type: post
  ClusterOperationStatus:
    properties:
      details:
        description: This is a default description.
        type: post
      innerState:
        description: This is a default description.
        type: post
      state:
        description: This is a default description.
        type: post
      stateStartTime:
        description: This is a default description.
        type: post
  ClusterStatus:
    properties:
      detail:
        description: This is a default description.
        type: post
      state:
        description: This is a default description.
        type: post
      stateStartTime:
        description: This is a default description.
        type: post
  DiagnoseClusterOutputLocation:
    properties:
      outputUri:
        description: This is a default description.
        type: post
  DiagnoseClusterRequest:
    properties: []
  DiagnoseClusterResults:
    properties:
      outputUri:
        description: This is a default description.
        type: post
  DiskConfig:
    properties:
      bootDiskSizeGb:
        description: This is a default description.
        type: post
      numLocalSsds:
        description: This is a default description.
        type: post
  Empty:
    properties: []
  GceClusterConfig:
    properties:
      internalIpOnly:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      networkUri:
        description: This is a default description.
        type: post
      serviceAccount:
        description: This is a default description.
        type: post
      serviceAccountScopes:
        description: This is a default description.
        type: post
      subnetworkUri:
        description: This is a default description.
        type: post
      tags:
        description: This is a default description.
        type: post
      zoneUri:
        description: This is a default description.
        type: post
  HadoopJob:
    properties:
      archiveUris:
        description: This is a default description.
        type: post
      args:
        description: This is a default description.
        type: post
      fileUris:
        description: This is a default description.
        type: post
      jarFileUris:
        description: This is a default description.
        type: post
      mainClass:
        description: This is a default description.
        type: post
      mainJarFileUri:
        description: This is a default description.
        type: post
      properties:
        description: This is a default description.
        type: post
  HiveJob:
    properties:
      continueOnFailure:
        description: This is a default description.
        type: post
      jarFileUris:
        description: This is a default description.
        type: post
      properties:
        description: This is a default description.
        type: post
      queryFileUri:
        description: This is a default description.
        type: post
      scriptVariables:
        description: This is a default description.
        type: post
  InstanceGroupConfig:
    properties:
      accelerators:
        description: This is a default description.
        type: post
      imageUri:
        description: This is a default description.
        type: post
      instanceNames:
        description: This is a default description.
        type: post
      isPreemptible:
        description: This is a default description.
        type: post
      machineTypeUri:
        description: This is a default description.
        type: post
      numInstances:
        description: This is a default description.
        type: post
  Job:
    properties:
      driverControlFilesUri:
        description: This is a default description.
        type: post
      driverOutputResourceUri:
        description: This is a default description.
        type: post
      labels:
        description: This is a default description.
        type: post
      statusHistory:
        description: This is a default description.
        type: post
      yarnApplications:
        description: This is a default description.
        type: post
  JobPlacement:
    properties:
      clusterName:
        description: This is a default description.
        type: post
      clusterUuid:
        description: This is a default description.
        type: post
  JobReference:
    properties:
      jobId:
        description: This is a default description.
        type: post
      projectId:
        description: This is a default description.
        type: post
  JobScheduling:
    properties:
      maxFailuresPerHour:
        description: This is a default description.
        type: post
  JobStatus:
    properties:
      details:
        description: This is a default description.
        type: post
      state:
        description: This is a default description.
        type: post
      stateStartTime:
        description: This is a default description.
        type: post
  ListClustersResponse:
    properties:
      clusters:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  ListJobsResponse:
    properties:
      jobs:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
  ListOperationsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      operations:
        description: This is a default description.
        type: post
  LoggingConfig:
    properties:
      driverLogLevels:
        description: This is a default description.
        type: post
  ManagedGroupConfig:
    properties:
      instanceGroupManagerName:
        description: This is a default description.
        type: post
      instanceTemplateName:
        description: This is a default description.
        type: post
  NodeInitializationAction:
    properties:
      executableFile:
        description: This is a default description.
        type: post
      executionTimeout:
        description: This is a default description.
        type: post
  Operation:
    properties:
      done:
        description: This is a default description.
        type: post
      metadata:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      response:
        description: This is a default description.
        type: post
  OperationMetadata:
    properties:
      clusterName:
        description: This is a default description.
        type: post
      clusterUuid:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
      endTime:
        description: This is a default description.
        type: post
      innerState:
        description: This is a default description.
        type: post
      insertTime:
        description: This is a default description.
        type: post
      operationType:
        description: This is a default description.
        type: post
      startTime:
        description: This is a default description.
        type: post
      state:
        description: This is a default description.
        type: post
  OperationStatus:
    properties:
      details:
        description: This is a default description.
        type: post
      innerState:
        description: This is a default description.
        type: post
      state:
        description: This is a default description.
        type: post
      stateStartTime:
        description: This is a default description.
        type: post
  PigJob:
    properties:
      continueOnFailure:
        description: This is a default description.
        type: post
      jarFileUris:
        description: This is a default description.
        type: post
      properties:
        description: This is a default description.
        type: post
      queryFileUri:
        description: This is a default description.
        type: post
      scriptVariables:
        description: This is a default description.
        type: post
  PySparkJob:
    properties:
      archiveUris:
        description: This is a default description.
        type: post
      args:
        description: This is a default description.
        type: post
      fileUris:
        description: This is a default description.
        type: post
      jarFileUris:
        description: This is a default description.
        type: post
      mainPythonFileUri:
        description: This is a default description.
        type: post
      properties:
        description: This is a default description.
        type: post
      pythonFileUris:
        description: This is a default description.
        type: post
  QueryList:
    properties:
      queries:
        description: This is a default description.
        type: post
  SoftwareConfig:
    properties:
      imageVersion:
        description: This is a default description.
        type: post
      properties:
        description: This is a default description.
        type: post
  SparkJob:
    properties:
      archiveUris:
        description: This is a default description.
        type: post
      args:
        description: This is a default description.
        type: post
      fileUris:
        description: This is a default description.
        type: post
      jarFileUris:
        description: This is a default description.
        type: post
      mainClass:
        description: This is a default description.
        type: post
      mainJarFileUri:
        description: This is a default description.
        type: post
      properties:
        description: This is a default description.
        type: post
  SparkSqlJob:
    properties:
      jarFileUris:
        description: This is a default description.
        type: post
      properties:
        description: This is a default description.
        type: post
      queryFileUri:
        description: This is a default description.
        type: post
      scriptVariables:
        description: This is a default description.
        type: post
  Status:
    properties:
      code:
        description: This is a default description.
        type: post
      details:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  SubmitJobRequest:
    properties: []
  YarnApplication:
    properties:
      name:
        description: This is a default description.
        type: post
      progress:
        description: This is a default description.
        type: post
      state:
        description: This is a default description.
        type: post
      trackingUrl:
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