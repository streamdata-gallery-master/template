---
swagger: "2.0"
info:
  title: CdnManagementClient
  description: Use these APIs to manage Azure CDN resources through the Azure Resource
    Manager. You must make sure that requests made to these resources are secure.
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
  /subscriptions/{subscriptionId}/providers/Microsoft.Cdn/profiles:
    get:
      summary: Profiles List
      description: Lists all of the CDN profiles within an Azure subscription
      operationId: Profiles_List
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - profile
definitions:
  Profile:
    properties: []
  ProfileProperties:
    properties:
      resourceState:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  ProfileListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ProfileUpdateParameters:
    properties:
      tags:
        description: This is a default description.
        type: get
  SsoUri:
    properties:
      ssoUriValue:
        description: This is a default description.
        type: get
  Endpoint:
    properties: []
  EndpointProperties:
    properties:
      hostName:
        description: This is a default description.
        type: get
      origins:
        description: This is a default description.
        type: get
      resourceState:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  EndpointListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  EndpointUpdateParameters:
    properties:
      tags:
        description: This is a default description.
        type: get
  EndpointPropertiesUpdateParameters:
    properties:
      originHostHeader:
        description: This is a default description.
        type: get
      originPath:
        description: This is a default description.
        type: get
      contentTypesToCompress:
        description: This is a default description.
        type: get
      isCompressionEnabled:
        description: This is a default description.
        type: get
      isHttpAllowed:
        description: This is a default description.
        type: get
      isHttpsAllowed:
        description: This is a default description.
        type: get
      optimizationType:
        description: This is a default description.
        type: get
      geoFilters:
        description: This is a default description.
        type: get
  DeepCreatedOrigin:
    properties:
      name:
        description: This is a default description.
        type: get
  DeepCreatedOriginProperties:
    properties:
      hostName:
        description: This is a default description.
        type: get
      httpPort:
        description: This is a default description.
        type: get
      httpsPort:
        description: This is a default description.
        type: get
  GeoFilter:
    properties:
      relativePath:
        description: This is a default description.
        type: get
      action:
        description: This is a default description.
        type: get
      countryCodes:
        description: This is a default description.
        type: get
  PurgeParameters:
    properties:
      contentPaths:
        description: This is a default description.
        type: get
  LoadParameters:
    properties:
      contentPaths:
        description: This is a default description.
        type: get
  Origin:
    properties: []
  OriginProperties:
    properties:
      hostName:
        description: This is a default description.
        type: get
      httpPort:
        description: This is a default description.
        type: get
      httpsPort:
        description: This is a default description.
        type: get
      resourceState:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  OriginUpdateParameters:
    properties: []
  OriginPropertiesParameters:
    properties:
      hostName:
        description: This is a default description.
        type: get
      httpPort:
        description: This is a default description.
        type: get
      httpsPort:
        description: This is a default description.
        type: get
  OriginListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  CustomDomain:
    properties: []
  CustomDomainProperties:
    properties:
      hostName:
        description: This is a default description.
        type: get
      resourceState:
        description: This is a default description.
        type: get
      customHttpsProvisioningState:
        description: This is a default description.
        type: get
      validationData:
        description: This is a default description.
        type: get
      provisioningState:
        description: This is a default description.
        type: get
  CustomDomainParameters:
    properties: []
  CustomDomainPropertiesParameters:
    properties:
      hostName:
        description: This is a default description.
        type: get
  CustomDomainListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ValidateCustomDomainInput:
    properties:
      hostName:
        description: This is a default description.
        type: get
  ValidateCustomDomainOutput:
    properties:
      customDomainValidated:
        description: This is a default description.
        type: get
      reason:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  CheckNameAvailabilityInput:
    properties:
      name:
        description: This is a default description.
        type: get
  CheckNameAvailabilityOutput:
    properties:
      nameAvailable:
        description: This is a default description.
        type: get
      reason:
        description: This is a default description.
        type: get
      message:
        description: This is a default description.
        type: get
  ResourceUsageListResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  ResourceUsage:
    properties:
      resourceType:
        description: This is a default description.
        type: get
      unit:
        description: This is a default description.
        type: get
      currentValue:
        description: This is a default description.
        type: get
      limit:
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
  EdgenodeResult:
    properties:
      value:
        description: This is a default description.
        type: get
      nextLink:
        description: This is a default description.
        type: get
  EdgeNode:
    properties: []
  EdgeNodeProperties:
    properties:
      ipAddressGroups:
        description: This is a default description.
        type: get
  IpAddressGroup:
    properties:
      deliveryRegion:
        description: This is a default description.
        type: get
      ipv4Addresses:
        description: This is a default description.
        type: get
      ipv6Addresses:
        description: This is a default description.
        type: get
  cidrIpAddress:
    properties:
      baseIpAddress:
        description: This is a default description.
        type: get
      prefixLength:
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
  Sku:
    properties:
      name:
        description: This is a default description.
        type: get
  ErrorResponse:
    properties:
      code:
        description: This is a default description.
        type: get
      message:
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