---
swagger: "2.0"
info:
  title: Google Play EMM
  description: Manages the deployment of apps to Android for Work users.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /androidenterprise/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /enterprises/{enterpriseId}/users/{userId}:
    get:
      summary: Get User
      description: Retrieves a user's details
      operationId: androidenterprise.users.get
      parameters:
      - in: path
        name: enterpriseId
        description: The ID of the enterprise
      - in: path
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - user
definitions:
  Administrator:
    properties:
      email:
        description: This is a default description.
        type: parameters
  AdministratorWebToken:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      token:
        description: This is a default description.
        type: parameters
  AdministratorWebTokenSpec:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      parent:
        description: This is a default description.
        type: parameters
      permission:
        description: This is a default description.
        type: parameters
  AppRestrictionsSchema:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      restrictions:
        description: This is a default description.
        type: parameters
  AppRestrictionsSchemaChangeEvent:
    properties:
      productId:
        description: This is a default description.
        type: parameters
  AppRestrictionsSchemaRestriction:
    properties:
      description:
        description: This is a default description.
        type: parameters
      entry:
        description: This is a default description.
        type: parameters
      entryValue:
        description: This is a default description.
        type: parameters
      key:
        description: This is a default description.
        type: parameters
      nestedRestriction:
        description: This is a default description.
        type: parameters
      restrictionType:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
  AppRestrictionsSchemaRestrictionRestrictionValue:
    properties:
      type:
        description: This is a default description.
        type: parameters
      valueBool:
        description: This is a default description.
        type: parameters
      valueInteger:
        description: This is a default description.
        type: parameters
      valueMultiselect:
        description: This is a default description.
        type: parameters
      valueString:
        description: This is a default description.
        type: parameters
  AppUpdateEvent:
    properties:
      productId:
        description: This is a default description.
        type: parameters
  AppVersion:
    properties:
      versionCode:
        description: This is a default description.
        type: parameters
      versionString:
        description: This is a default description.
        type: parameters
  ApprovalUrlInfo:
    properties:
      approvalUrl:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AuthenticationToken:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      token:
        description: This is a default description.
        type: parameters
  Device:
    properties:
      androidId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      managementType:
        description: This is a default description.
        type: parameters
  DeviceState:
    properties:
      accountState:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  DevicesListResponse:
    properties:
      device:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Enterprise:
    properties:
      administrator:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      primaryDomain:
        description: This is a default description.
        type: parameters
  EnterpriseAccount:
    properties:
      accountEmail:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  EnterprisesListResponse:
    properties:
      enterprise:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  EnterprisesSendTestPushNotificationResponse:
    properties:
      messageId:
        description: This is a default description.
        type: parameters
      topicName:
        description: This is a default description.
        type: parameters
  Entitlement:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
  EntitlementsListResponse:
    properties:
      entitlement:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  GroupLicense:
    properties:
      acquisitionKind:
        description: This is a default description.
        type: parameters
      approval:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      numProvisioned:
        description: This is a default description.
        type: parameters
      numPurchased:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
  GroupLicenseUsersListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      user:
        description: This is a default description.
        type: parameters
  GroupLicensesListResponse:
    properties:
      groupLicense:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Install:
    properties:
      installState:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
      versionCode:
        description: This is a default description.
        type: parameters
  InstallFailureEvent:
    properties:
      deviceId:
        description: This is a default description.
        type: parameters
      failureDetails:
        description: This is a default description.
        type: parameters
      failureReason:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
      userId:
        description: This is a default description.
        type: parameters
  InstallsListResponse:
    properties:
      install:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  LocalizedText:
    properties:
      locale:
        description: This is a default description.
        type: parameters
      text:
        description: This is a default description.
        type: parameters
  ManagedConfiguration:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      managedProperty:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
  ManagedConfigurationsForDeviceListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      managedConfigurationForDevice:
        description: This is a default description.
        type: parameters
  ManagedConfigurationsForUserListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      managedConfigurationForUser:
        description: This is a default description.
        type: parameters
  ManagedProperty:
    properties:
      key:
        description: This is a default description.
        type: parameters
      valueBool:
        description: This is a default description.
        type: parameters
      valueBundleArray:
        description: This is a default description.
        type: parameters
      valueInteger:
        description: This is a default description.
        type: parameters
      valueString:
        description: This is a default description.
        type: parameters
      valueStringArray:
        description: This is a default description.
        type: parameters
  ManagedPropertyBundle:
    properties:
      managedProperty:
        description: This is a default description.
        type: parameters
  NewDeviceEvent:
    properties:
      deviceId:
        description: This is a default description.
        type: parameters
      managementType:
        description: This is a default description.
        type: parameters
      userId:
        description: This is a default description.
        type: parameters
  NewPermissionsEvent:
    properties:
      approvedPermissions:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
      requestedPermissions:
        description: This is a default description.
        type: parameters
  Notification:
    properties:
      enterpriseId:
        description: This is a default description.
        type: parameters
      timestampMillis:
        description: This is a default description.
        type: parameters
  NotificationSet:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      notification:
        description: This is a default description.
        type: parameters
      notificationSetId:
        description: This is a default description.
        type: parameters
  PageInfo:
    properties:
      resultPerPage:
        description: This is a default description.
        type: parameters
      startIndex:
        description: This is a default description.
        type: parameters
      totalResults:
        description: This is a default description.
        type: parameters
  Permission:
    properties:
      description:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      permissionId:
        description: This is a default description.
        type: parameters
  Product:
    properties:
      appVersion:
        description: This is a default description.
        type: parameters
      authorName:
        description: This is a default description.
        type: parameters
      detailsUrl:
        description: This is a default description.
        type: parameters
      distributionChannel:
        description: This is a default description.
        type: parameters
      iconUrl:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
      productPricing:
        description: This is a default description.
        type: parameters
      requiresContainerApp:
        description: This is a default description.
        type: parameters
      smallIconUrl:
        description: This is a default description.
        type: parameters
  ProductApprovalEvent:
    properties:
      approved:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
  ProductAvailabilityChangeEvent:
    properties:
      availabilityStatus:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
  ProductPermission:
    properties:
      permissionId:
        description: This is a default description.
        type: parameters
      state:
        description: This is a default description.
        type: parameters
  ProductPermissions:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      permission:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
  ProductSet:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
      productSetBehavior:
        description: This is a default description.
        type: parameters
  ProductsApproveRequest:
    properties: []
  ProductsGenerateApprovalUrlResponse:
    properties:
      url:
        description: This is a default description.
        type: parameters
  ProductsListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      product:
        description: This is a default description.
        type: parameters
  ServiceAccount:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
  ServiceAccountKey:
    properties:
      data:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      publicData:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  ServiceAccountKeysListResponse:
    properties:
      serviceAccountKey:
        description: This is a default description.
        type: parameters
  SignupInfo:
    properties:
      completionToken:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      url:
        description: This is a default description.
        type: parameters
  StoreCluster:
    properties:
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      orderInPage:
        description: This is a default description.
        type: parameters
      productId:
        description: This is a default description.
        type: parameters
  StoreLayout:
    properties:
      homepageId:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      storeLayoutType:
        description: This is a default description.
        type: parameters
  StoreLayoutClustersListResponse:
    properties:
      cluster:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  StoreLayoutPagesListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      page:
        description: This is a default description.
        type: parameters
  StorePage:
    properties:
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      link:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
  TokenPagination:
    properties:
      nextPageToken:
        description: This is a default description.
        type: parameters
      previousPageToken:
        description: This is a default description.
        type: parameters
  User:
    properties:
      accountIdentifier:
        description: This is a default description.
        type: parameters
      accountType:
        description: This is a default description.
        type: parameters
      displayName:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      managementType:
        description: This is a default description.
        type: parameters
      primaryEmail:
        description: This is a default description.
        type: parameters
  UserToken:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      token:
        description: This is a default description.
        type: parameters
      userId:
        description: This is a default description.
        type: parameters
  UsersListResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      user:
        description: This is a default description.
        type: parameters
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