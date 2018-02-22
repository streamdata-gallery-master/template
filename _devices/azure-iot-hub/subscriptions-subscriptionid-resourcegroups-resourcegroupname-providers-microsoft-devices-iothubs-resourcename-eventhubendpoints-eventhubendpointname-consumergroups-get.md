---
swagger: "2.0"
info:
  title: iotHubClient
  description: Use this API to manage the IoT hubs in your subscription.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Devices/IotHubs/{resourceName}/eventHubEndpoints/{eventHubEndpointName}/ConsumerGroups
  : get:
      summary: Iot Hub Resource List Event Hub Consumer Groups
      description: Get a list of the consumer groups in the Event Hub-compatible device-to-cloud
        endpoint in an IoT hub
      operationId: IotHubResource_ListEventHubConsumerGroups
      parameters:
      - in: path
        name: eventHubEndpointName
        description: The name of the Event Hub-compatible endpoint
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group that contains the IoT hub
      - in: path
        name: resourceName
        description: The name of the IoT hub
      responses:
        200:
          description: OK
      tags:
      - iot hub resource event hub consumer groups
definitions:
  SharedAccessSignatureAuthorizationRule:
    properties:
      keyName:
        description: This is a default description.
        type: post
      primaryKey:
        description: This is a default description.
        type: post
      secondaryKey:
        description: This is a default description.
        type: post
      rights:
        description: This is a default description.
        type: post
  IotHubProperties:
    properties:
      authorizationPolicies:
        description: This is a default description.
        type: post
      ipFilterRules:
        description: This is a default description.
        type: post
      provisioningState:
        description: This is a default description.
        type: post
      hostName:
        description: This is a default description.
        type: post
      eventHubEndpoints:
        description: This is a default description.
        type: post
      storageEndpoints:
        description: This is a default description.
        type: post
      messagingEndpoints:
        description: This is a default description.
        type: post
      enableFileUploadNotifications:
        description: This is a default description.
        type: post
      comments:
        description: This is a default description.
        type: post
      features:
        description: This is a default description.
        type: post
  IotHubSkuInfo:
    properties:
      name:
        description: This is a default description.
        type: post
      tier:
        description: This is a default description.
        type: post
      capacity:
        description: This is a default description.
        type: post
  EventHubProperties:
    properties:
      retentionTimeInDays:
        description: This is a default description.
        type: post
      partitionCount:
        description: This is a default description.
        type: post
      partitionIds:
        description: This is a default description.
        type: post
      path:
        description: This is a default description.
        type: post
      endpoint:
        description: This is a default description.
        type: post
  StorageEndpointProperties:
    properties:
      sasTtlAsIso8601:
        description: This is a default description.
        type: post
      connectionString:
        description: This is a default description.
        type: post
      containerName:
        description: This is a default description.
        type: post
  MessagingEndpointProperties:
    properties:
      lockDurationAsIso8601:
        description: This is a default description.
        type: post
      ttlAsIso8601:
        description: This is a default description.
        type: post
      maxDeliveryCount:
        description: This is a default description.
        type: post
  CloudToDeviceProperties:
    properties:
      maxDeliveryCount:
        description: This is a default description.
        type: post
      defaultTtlAsIso8601:
        description: This is a default description.
        type: post
  OperationsMonitoringProperties:
    properties:
      events:
        description: This is a default description.
        type: post
  IpFilterRule:
    properties:
      filterName:
        description: This is a default description.
        type: post
      action:
        description: This is a default description.
        type: post
      ipMask:
        description: This is a default description.
        type: post
  FeedbackProperties:
    properties:
      lockDurationAsIso8601:
        description: This is a default description.
        type: post
      ttlAsIso8601:
        description: This is a default description.
        type: post
      maxDeliveryCount:
        description: This is a default description.
        type: post
  IotHubDescription:
    properties:
      subscriptionid:
        description: This is a default description.
        type: post
      resourcegroup:
        description: This is a default description.
        type: post
      etag:
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
  SharedAccessSignatureAuthorizationRuleListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  ErrorDetails:
    properties:
      Code:
        description: This is a default description.
        type: post
      HttpStatusCode:
        description: This is a default description.
        type: post
      Message:
        description: This is a default description.
        type: post
      Details:
        description: This is a default description.
        type: post
  IotHubQuotaMetricInfoListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  RegistryStatistics:
    properties:
      totalDeviceCount:
        description: This is a default description.
        type: post
      enabledDeviceCount:
        description: This is a default description.
        type: post
      disabledDeviceCount:
        description: This is a default description.
        type: post
  JobResponseListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  IotHubSkuDescription:
    properties:
      resourceType:
        description: This is a default description.
        type: post
  IotHubCapacity:
    properties:
      minimum:
        description: This is a default description.
        type: post
      maximum:
        description: This is a default description.
        type: post
      default:
        description: This is a default description.
        type: post
      scaleType:
        description: This is a default description.
        type: post
  EventHubConsumerGroupsListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  EventHubConsumerGroupInfo:
    properties:
      tags:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  IotHubSkuDescriptionListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  JobResponse:
    properties:
      jobId:
        description: This is a default description.
        type: post
      startTimeUtc:
        description: This is a default description.
        type: post
      endTimeUtc:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      failureReason:
        description: This is a default description.
        type: post
      statusMessage:
        description: This is a default description.
        type: post
      parentJobId:
        description: This is a default description.
        type: post
  IotHubDescriptionListResult:
    properties:
      value:
        description: This is a default description.
        type: post
      nextLink:
        description: This is a default description.
        type: post
  IotHubQuotaMetricInfo:
    properties:
      Name:
        description: This is a default description.
        type: post
      CurrentValue:
        description: This is a default description.
        type: post
      MaxValue:
        description: This is a default description.
        type: post
  OperationInputs:
    properties:
      Name:
        description: This is a default description.
        type: post
  IotHubNameAvailabilityInfo:
    properties:
      nameAvailable:
        description: This is a default description.
        type: post
      reason:
        description: This is a default description.
        type: post
      message:
        description: This is a default description.
        type: post
  ExportDevicesRequest:
    properties:
      ExportBlobContainerUri:
        description: This is a default description.
        type: post
      ExcludeKeys:
        description: This is a default description.
        type: post
  ImportDevicesRequest:
    properties:
      InputBlobContainerUri:
        description: This is a default description.
        type: post
      OutputBlobContainerUri:
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