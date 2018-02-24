---
swagger: "2.0"
info:
  title: Azure ML Web Services Management Client
  description: These APIs allow end users to operate on Azure Machine Learning Web
    Services resources. They support the following operations:&lt;ul&gt;&lt;li&gt;Create
    or update a web service&lt;/li&gt;&lt;li&gt;Get a web service&lt;/li&gt;&lt;li&gt;Patch
    a web service&lt;/li&gt;&lt;li&gt;Delete a web service&lt;/li&gt;&lt;li&gt;Get
    All Web Services in a Resource Group &lt;/li&gt;&lt;li&gt;Get All Web Services
    in a Subscription&lt;/li&gt;&lt;li&gt;Get Web Services Keys&lt;/li&gt;&lt;/ul&gt;
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.MachineLearning/webServices/{webServiceName}
  : put:
      summary: Web Services Create Or Update
      description: Create or update a web service
      operationId: WebServices_CreateOrUpdate
      parameters:
      - in: body
        name: createOrUpdatePayload
        description: The payload that is used to create or update the web service
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - web services
definitions:
  Resource:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      location:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      tags:
        description: This is a default description.
        type: get
  WebService:
    properties: []
  WebServiceProperties:
    properties:
      title:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      createdOn:
        description: This is a default description.
        type: get
      modifiedOn:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
      readOnly:
        description: This is a default description.
        type: get
      swaggerLocation:
        description: This is a default description.
        type: get
      exposeSampleData:
        description: This is a default description.
        type: get
      assets:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
  WebServicePropertiesForGraph:
    properties: []
  WebServiceKeys:
    properties:
      primary:
        description: This is a default description.
        type: get
      secondary:
        description: This is a default description.
        type: get
  PaginatedWebServicesList:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  RealtimeConfiguration:
    properties:
      maxConcurrentCalls:
        description: This is a default description.
        type: get
  DiagnosticsConfiguration:
    properties:
      level:
        description: This is a default description.
        type: get
      expiry:
        description: This is a default description.
        type: get
  StorageAccount:
    properties:
      name:
        description: This is a default description.
        type: get
      key:
        description: This is a default description.
        type: get
  MachineLearningWorkspace:
    properties:
      id:
        description: This is a default description.
        type: get
  CommitmentPlan:
    properties:
      id:
        description: This is a default description.
        type: get
  ServiceInputOutputSpecification:
    properties:
      title:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      properties:
        description: This is a default description.
        type: get
  TableSpecification:
    properties:
      title:
        description: This is a default description.
        type: get
      description:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      format:
        description: This is a default description.
        type: get
      properties:
        description: This is a default description.
        type: get
  ColumnSpecification:
    properties:
      type:
        description: This is a default description.
        type: get
      format:
        description: This is a default description.
        type: get
      enum:
        description: This is a default description.
        type: get
      x-ms-isnullable:
        description: This is a default description.
        type: get
      x-ms-isordered:
        description: This is a default description.
        type: get
  ExampleRequest:
    properties:
      inputs:
        description: This is a default description.
        type: get
      globalParameters:
        description: This is a default description.
        type: get
  AssetItem:
    properties:
      name:
        description: This is a default description.
        type: get
      id:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      inputPorts:
        description: This is a default description.
        type: get
      outputPorts:
        description: This is a default description.
        type: get
      metadata:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
  BlobLocation:
    properties:
      uri:
        description: This is a default description.
        type: get
      credentials:
        description: This is a default description.
        type: get
  ModuleAssetParameter:
    properties:
      name:
        description: This is a default description.
        type: get
      parameterType:
        description: This is a default description.
        type: get
      modeValuesInfo:
        description: This is a default description.
        type: get
  ModeValueInfo:
    properties:
      interfaceString:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
  InputPort:
    properties:
      type:
        description: This is a default description.
        type: get
  OutputPort:
    properties:
      type:
        description: This is a default description.
        type: get
  GraphPackage:
    properties:
      nodes:
        description: This is a default description.
        type: get
      edges:
        description: This is a default description.
        type: get
      graphParameters:
        description: This is a default description.
        type: get
  GraphNode:
    properties:
      assetId:
        description: This is a default description.
        type: get
      inputId:
        description: This is a default description.
        type: get
      outputId:
        description: This is a default description.
        type: get
      parameters:
        description: This is a default description.
        type: get
  GraphEdge:
    properties:
      sourceNodeId:
        description: This is a default description.
        type: get
      sourcePortId:
        description: This is a default description.
        type: get
      targetNodeId:
        description: This is a default description.
        type: get
      targetPortId:
        description: This is a default description.
        type: get
  GraphParameter:
    properties:
      description:
        description: This is a default description.
        type: get
      type:
        description: This is a default description.
        type: get
      links:
        description: This is a default description.
        type: get
  GraphParameterLink:
    properties:
      nodeId:
        description: This is a default description.
        type: get
      parameterKey:
        description: This is a default description.
        type: get
  WebServiceParameter:
    properties:
      value:
        description: This is a default description.
        type: get
      certificateThumbprint:
        description: This is a default description.
        type: get
  AsyncOperationStatus:
    properties:
      id:
        description: This is a default description.
        type: get
      name:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
      startTime:
        description: This is a default description.
        type: get
      endTime:
        description: This is a default description.
        type: get
      percentComplete:
        description: This is a default description.
        type: get
  AsyncOperationErrorInfo:
    properties:
      code:
        description: This is a default description.
        type: get
      target:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
      details:
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