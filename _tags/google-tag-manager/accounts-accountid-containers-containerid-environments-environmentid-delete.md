---
swagger: "2.0"
info:
  title: Tag Manager
  description: Accesses Tag Manager accounts and containers.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tagmanager/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/containers/{containerId}/environments/{environmentId}:
    delete:
      summary: Delete GTM Environment
      description: Deletes a GTM Environment
      operationId: tagmanager.accounts.containers.environments.delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      responses:
        200:
          description: OK
      tags:
      - gtm environment
definitions:
  Account:
    properties:
      accountId:
        description: This is a default description.
        type: put
      fingerprint:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      shareData:
        description: This is a default description.
        type: put
  AccountAccess:
    properties:
      permission:
        description: This is a default description.
        type: put
  Condition:
    properties:
      parameter:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  Container:
    properties:
      accountId:
        description: This is a default description.
        type: put
      containerId:
        description: This is a default description.
        type: put
      domainName:
        description: This is a default description.
        type: put
      enabledBuiltInVariable:
        description: This is a default description.
        type: put
      fingerprint:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      notes:
        description: This is a default description.
        type: put
      publicId:
        description: This is a default description.
        type: put
      timeZoneCountryId:
        description: This is a default description.
        type: put
      timeZoneId:
        description: This is a default description.
        type: put
  ContainerAccess:
    properties:
      containerId:
        description: This is a default description.
        type: put
      permission:
        description: This is a default description.
        type: put
  ContainerVersion:
    properties:
      accountId:
        description: This is a default description.
        type: put
      containerId:
        description: This is a default description.
        type: put
      containerVersionId:
        description: This is a default description.
        type: put
      deleted:
        description: This is a default description.
        type: put
      fingerprint:
        description: This is a default description.
        type: put
      folder:
        description: This is a default description.
        type: put
      macro:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      notes:
        description: This is a default description.
        type: put
      rule:
        description: This is a default description.
        type: put
  ContainerVersionHeader:
    properties:
      accountId:
        description: This is a default description.
        type: put
      containerId:
        description: This is a default description.
        type: put
      containerVersionId:
        description: This is a default description.
        type: put
      deleted:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      numMacros:
        description: This is a default description.
        type: put
      numRules:
        description: This is a default description.
        type: put
      numTags:
        description: This is a default description.
        type: put
      numTriggers:
        description: This is a default description.
        type: put
      numVariables:
        description: This is a default description.
        type: put
  CreateContainerVersionRequestVersionOptions:
    properties:
      name:
        description: This is a default description.
        type: put
      notes:
        description: This is a default description.
        type: put
      quickPreview:
        description: This is a default description.
        type: put
  CreateContainerVersionResponse:
    properties:
      compilerError:
        description: This is a default description.
        type: put
  Environment:
    properties:
      accountId:
        description: This is a default description.
        type: put
      authorizationCode:
        description: This is a default description.
        type: put
      authorizationTimestampMs:
        description: This is a default description.
        type: put
      containerId:
        description: This is a default description.
        type: put
      containerVersionId:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      enableDebug:
        description: This is a default description.
        type: put
      environmentId:
        description: This is a default description.
        type: put
      fingerprint:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
  Folder:
    properties:
      accountId:
        description: This is a default description.
        type: put
      containerId:
        description: This is a default description.
        type: put
      fingerprint:
        description: This is a default description.
        type: put
      folderId:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
  FolderEntities:
    properties:
      tag:
        description: This is a default description.
        type: put
      trigger:
        description: This is a default description.
        type: put
      variable:
        description: This is a default description.
        type: put
  ListAccountUsersResponse:
    properties:
      userAccess:
        description: This is a default description.
        type: put
  ListAccountsResponse:
    properties:
      accounts:
        description: This is a default description.
        type: put
  ListContainerVersionsResponse:
    properties:
      containerVersion:
        description: This is a default description.
        type: put
      containerVersionHeader:
        description: This is a default description.
        type: put
  ListContainersResponse:
    properties:
      containers:
        description: This is a default description.
        type: put
  ListEnvironmentsResponse:
    properties:
      environments:
        description: This is a default description.
        type: put
  ListFoldersResponse:
    properties:
      folders:
        description: This is a default description.
        type: put
  ListTagsResponse:
    properties:
      tags:
        description: This is a default description.
        type: put
  ListTriggersResponse:
    properties:
      triggers:
        description: This is a default description.
        type: put
  ListVariablesResponse:
    properties:
      variables:
        description: This is a default description.
        type: put
  Macro:
    properties:
      accountId:
        description: This is a default description.
        type: put
      containerId:
        description: This is a default description.
        type: put
      disablingRuleId:
        description: This is a default description.
        type: put
      enablingRuleId:
        description: This is a default description.
        type: put
      fingerprint:
        description: This is a default description.
        type: put
      macroId:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      notes:
        description: This is a default description.
        type: put
      parameter:
        description: This is a default description.
        type: put
      parentFolderId:
        description: This is a default description.
        type: put
  Parameter:
    properties:
      key:
        description: This is a default description.
        type: put
      list:
        description: This is a default description.
        type: put
      map:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      value:
        description: This is a default description.
        type: put
  PublishContainerVersionResponse:
    properties:
      compilerError:
        description: This is a default description.
        type: put
  Rule:
    properties:
      accountId:
        description: This is a default description.
        type: put
      condition:
        description: This is a default description.
        type: put
      containerId:
        description: This is a default description.
        type: put
      fingerprint:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      notes:
        description: This is a default description.
        type: put
      ruleId:
        description: This is a default description.
        type: put
  SetupTag:
    properties:
      stopOnSetupFailure:
        description: This is a default description.
        type: put
      tagName:
        description: This is a default description.
        type: put
  Tag:
    properties:
      accountId:
        description: This is a default description.
        type: put
      blockingRuleId:
        description: This is a default description.
        type: put
      blockingTriggerId:
        description: This is a default description.
        type: put
      containerId:
        description: This is a default description.
        type: put
      fingerprint:
        description: This is a default description.
        type: put
      firingRuleId:
        description: This is a default description.
        type: put
      firingTriggerId:
        description: This is a default description.
        type: put
      liveOnly:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      notes:
        description: This is a default description.
        type: put
  TeardownTag:
    properties:
      stopTeardownOnFailure:
        description: This is a default description.
        type: put
      tagName:
        description: This is a default description.
        type: put
  Trigger:
    properties:
      accountId:
        description: This is a default description.
        type: put
      autoEventFilter:
        description: This is a default description.
        type: put
      containerId:
        description: This is a default description.
        type: put
      customEventFilter:
        description: This is a default description.
        type: put
      filter:
        description: This is a default description.
        type: put
      fingerprint:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      parentFolderId:
        description: This is a default description.
        type: put
      triggerId:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  UserAccess:
    properties:
      accountId:
        description: This is a default description.
        type: put
      containerAccess:
        description: This is a default description.
        type: put
      emailAddress:
        description: This is a default description.
        type: put
      permissionId:
        description: This is a default description.
        type: put
  Variable:
    properties:
      accountId:
        description: This is a default description.
        type: put
      containerId:
        description: This is a default description.
        type: put
      disablingTriggerId:
        description: This is a default description.
        type: put
      enablingTriggerId:
        description: This is a default description.
        type: put
      fingerprint:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      notes:
        description: This is a default description.
        type: put
      parameter:
        description: This is a default description.
        type: put
      parentFolderId:
        description: This is a default description.
        type: put
      scheduleEndMs:
        description: This is a default description.
        type: put
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