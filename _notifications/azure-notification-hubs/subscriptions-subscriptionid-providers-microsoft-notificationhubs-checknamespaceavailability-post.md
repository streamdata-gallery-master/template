---
swagger: "2.0"
info:
  title: NotificationHubsManagementClient
  description: Azure NotificationHub client
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
  /subscriptions/{subscriptionId}/providers/Microsoft.NotificationHubs/checkNamespaceAvailability:
    post:
      summary: Namespaces Check Availability
      description: Checks the availability of the given service namespace across all
        Azure subscriptions
      operationId: Namespaces_CheckAvailability
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The namespace name
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - namespaces availability
definitions:
  CheckAvailabilityParameters:
    properties:
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      tags:
        description: This is a default description.
        type: post
      isAvailiable:
        description: This is a default description.
        type: post
  CheckAvailabilityResult:
    properties:
      isAvailiable:
        description: This is a default description.
        type: post
  NamespaceProperties:
    properties:
      name:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      region:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      createdAt:
        description: This is a default description.
        type: post
      serviceBusEndpoint:
        description: This is a default description.
        type: post
      subscriptionId:
        description: This is a default description.
        type: post
      scaleUnit:
        description: This is a default description.
        type: post
      enabled:
        description: This is a default description.
        type: post
      critical:
        description: This is a default description.
        type: post
  NamespaceCreateOrUpdateParameters:
    properties: []
  NamespacePatchParameters:
    properties:
      tags:
        description: This is a default description.
        type: post
  NamespaceResource:
    properties: []
  SharedAccessAuthorizationRuleProperties:
    properties:
      rights:
        description: This is a default description.
        type: post
  SharedAccessAuthorizationRuleCreateOrUpdateParameters:
    properties: []
  SharedAccessAuthorizationRuleResource:
    properties: []
  NamespaceListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  SharedAccessAuthorizationRuleListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ResourceListKeys:
    properties:
      primaryConnectionString:
        description: This is a default description.
        type: post
      secondaryConnectionString:
        description: This is a default description.
        type: post
      primaryKey:
        description: This is a default description.
        type: post
      secondaryKey:
        description: This is a default description.
        type: post
      keyName:
        description: This is a default description.
        type: post
  PolicykeyResource:
    properties:
      policyKey:
        description: This is a default description.
        type: post
  ApnsCredentialProperties:
    properties:
      apnsCertificate:
        description: This is a default description.
        type: post
      certificateKey:
        description: This is a default description.
        type: post
      endpoint:
        description: This is a default description.
        type: post
      thumbprint:
        description: This is a default description.
        type: post
  ApnsCredential:
    properties: []
  WnsCredentialProperties:
    properties:
      packageSid:
        description: This is a default description.
        type: post
      secretKey:
        description: This is a default description.
        type: post
      windowsLiveEndpoint:
        description: This is a default description.
        type: post
  WnsCredential:
    properties: []
  GcmCredentialProperties:
    properties:
      gcmEndpoint:
        description: This is a default description.
        type: post
      googleApiKey:
        description: This is a default description.
        type: post
  GcmCredential:
    properties: []
  MpnsCredentialProperties:
    properties:
      mpnsCertificate:
        description: This is a default description.
        type: post
      certificateKey:
        description: This is a default description.
        type: post
      thumbprint:
        description: This is a default description.
        type: post
  MpnsCredential:
    properties: []
  AdmCredentialProperties:
    properties:
      clientId:
        description: This is a default description.
        type: post
      clientSecret:
        description: This is a default description.
        type: post
      authTokenUrl:
        description: This is a default description.
        type: post
  AdmCredential:
    properties: []
  BaiduCredentialProperties:
    properties:
      baiduApiKey:
        description: This is a default description.
        type: post
      baiduEndPoint:
        description: This is a default description.
        type: post
      baiduSecretKey:
        description: This is a default description.
        type: post
  BaiduCredential:
    properties: []
  NotificationHubProperties:
    properties:
      name:
        description: This is a default description.
        type: post
      registrationTtl:
        description: This is a default description.
        type: post
      authorizationRules:
        description: This is a default description.
        type: post
  NotificationHubCreateOrUpdateParameters:
    properties: []
  NotificationHubResource:
    properties: []
  PnsCredentialsResource:
    properties: []
  PnsCredentialsProperties:
    properties: []
  NotificationHubListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  Resource:
    properties:
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
      location:
        description: This is a default description.
        type: post
      tags:
        description: This is a default description.
        type: post
  SubResource:
    properties:
      id:
        description: This is a default description.
        type: post
  Sku:
    properties:
      name:
        description: This is a default description.
        type: post
      tier:
        description: This is a default description.
        type: post
      size:
        description: This is a default description.
        type: post
      family:
        description: This is a default description.
        type: post
      capacity:
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