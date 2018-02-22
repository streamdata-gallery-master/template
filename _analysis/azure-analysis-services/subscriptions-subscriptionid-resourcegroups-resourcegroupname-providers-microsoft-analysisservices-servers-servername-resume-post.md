---
swagger: "2.0"
info:
  title: AzureAnalysisServices
  description: The Azure Analysis Services Web API provides a RESTful set of web services
    that enables users to create, retrieve, update, and delete Analysis Services servers
  version: "2016-05-16"
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.AnalysisServices/servers/{serverName}/resume
  : post:
      summary: Resume Server
      description: Resumes operation of the specified Analysis Services server instance
      operationId: Servers_Resume
      parameters:
      - in: query
        name: No Name
      - in: path
        name: serverName
        description: The name of the Analysis Services server
      responses:
        200:
          description: OK
      tags:
      - servers
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
  AnalysisServicesServer:
    properties: []
  AnalysisServicesServers:
    properties:
      value:
        description: This is a default description.
        type: get
  AnalysisServicesServerUpdateParameters:
    properties:
      tags:
        description: This is a default description.
        type: get
  AnalysisServicesServerProperties:
    properties:
      state:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
      serverFullName:
        description: This is a default description.
        type: get
  ResourceSku:
    properties:
      name:
        description: This is a default description.
        type: get
      tier:
        description: This is a default description.
        type: get
  AnalysisServicesServerMutableProperties:
    properties: []
  ServerAdministrators:
    properties:
      members:
        description: This is a default description.
        type: get
  BackupConfiguration:
    properties:
      storageAccount:
        description: This is a default description.
        type: get
      blobContainer:
        description: This is a default description.
        type: get
      accessKey:
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