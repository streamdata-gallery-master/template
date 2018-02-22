---
swagger: "2.0"
info:
  title: ContainerServiceClient
  description: The Container Service Client.
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
  /subscriptions/{subscriptionId}/providers/Microsoft.ContainerService/containerServices:
    get:
      summary: Container Services List
      description: Gets a list of container services in the specified subscription
      operationId: ContainerServices_List
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - container service
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
      location:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  ContainerServiceCustomProfile:
    properties:
      orchestrator:
        description: This is a default description.
        type: get
  ContainerServiceServicePrincipalProfile:
    properties:
      clientId:
        description: This is a default description.
        type: get
      secret:
        description: This is a default description.
        type: get
  ContainerServiceOrchestratorProfile:
    properties:
      orchestratorType:
        description: This is a default description.
        type: get
  ContainerServiceMasterProfile:
    properties:
      count:
        description: This is a default description.
        type: get
      dnsPrefix:
        description: This is a default description.
        type: get
      fqdn:
        description: This is a default description.
        type: get
  ContainerServiceAgentPoolProfile:
    properties:
      name:
        description: This is a default description.
        type: get
      count:
        description: This is a default description.
        type: get
      vmSize:
        description: This is a default description.
        type: get
      dnsPrefix:
        description: This is a default description.
        type: get
      fqdn:
        description: This is a default description.
        type: get
  ContainerServiceWindowsProfile:
    properties:
      adminUsername:
        description: This is a default description.
        type: get
      adminPassword:
        description: This is a default description.
        type: get
  ContainerServiceLinuxProfile:
    properties:
      adminUsername:
        description: This is a default description.
        type: get
  ContainerServiceSshConfiguration:
    properties:
      publicKeys:
        description: This is a default description.
        type: get
  ContainerServiceSshPublicKey:
    properties:
      keyData:
        description: This is a default description.
        type: get
  ContainerServiceDiagnosticsProfile:
    properties: []
  ContainerServiceVMDiagnostics:
    properties:
      enabled:
        description: This is a default description.
        type: get
      storageUri:
        description: This is a default description.
        type: get
  ContainerService:
    properties: []
  ContainerServiceListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ContainerServiceProperties:
    properties:
      provisioningState:
        description: This is a default description.
        type: get
      agentPoolProfiles:
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