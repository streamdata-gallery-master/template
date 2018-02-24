---
swagger: "2.0"
info:
  title: Application Insights API
  description: Application Insights (in preview) is an all-in-one telemetry solution
    that can help you detect issues, triage impact and solve problems in your web
    apps and services. It provides deep diagnostics and real-time insights while being
    a seamless part of your ALM processes through Visual Studio, Visual Studio Team
    Services, and Azure Diagnostics integrations. It supports ASP.NET, J2EE and most
    of the popular web technologies for web apps on Azure or on your own servers.
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
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/webtests:
    get:
      summary: Web Tests By Resource Group
      description: Get all Application Insights web tests defined within a specified
        resource group
      operationId: WebTests_ListByResourceGroup
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - web tests
definitions:
  ErrorResponse:
    properties:
      code:
        description: This is a default description.
        type: get
      message:
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
      location:
        description: This is a default description.
        type: patch
  TagsResource:
    properties: []
  ApplicationInsightsComponent:
    properties:
      kind:
        description: This is a default description.
        type: patch
  ApplicationInsightsComponentProperties:
    properties:
      ApplicationId:
        description: This is a default description.
        type: patch
      AppId:
        description: This is a default description.
        type: patch
      Application_Type:
        description: This is a default description.
        type: patch
      Flow_Type:
        description: This is a default description.
        type: patch
      Request_Source:
        description: This is a default description.
        type: patch
      InstrumentationKey:
        description: This is a default description.
        type: patch
      CreationDate:
        description: This is a default description.
        type: patch
      TenantId:
        description: This is a default description.
        type: patch
      HockeyAppId:
        description: This is a default description.
        type: patch
      HockeyAppToken:
        description: This is a default description.
        type: patch
  ApplicationInsightsComponentListResult:
    properties:
      value:
        description: This is a default description.
        type: patch
      nextLink:
        description: This is a default description.
        type: patch
  webTestListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  WebTest:
    properties:
      kind:
        description: This is a default description.
        type: get
  WebTestProperties:
    properties:
      SyntheticMonitorId:
        description: This is a default description.
        type: get
      Name:
        description: This is a default description.
        type: get
      Description:
        description: This is a default description.
        type: get
      Enabled:
        description: This is a default description.
        type: get
      Frequency:
        description: This is a default description.
        type: get
      Timeout:
        description: This is a default description.
        type: get
      Kind:
        description: This is a default description.
        type: get
      RetryEnabled:
        description: This is a default description.
        type: get
      Locations:
        description: This is a default description.
        type: get
      Configuration:
        description: This is a default description.
        type: get
  WebTestGeolocation:
    properties:
      Id:
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