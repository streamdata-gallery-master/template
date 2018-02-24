---
swagger: "2.0"
info:
  title: DocumentDB
  description: Azure DocumentDB Database Service Resource Provider REST API
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DocumentDB/databaseAccounts/{accountName}/failoverPriorityChange
  : post:
      summary: Database Accounts Failover Priority Change
      description: Changes the failover priority for the Azure DocumentDB database
        account
      operationId: DatabaseAccounts_FailoverPriorityChange
      parameters:
      - in: body
        name: failoverParameters
        description: The new failover policies for the database account
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - database accounts failover priority change
definitions:
  DatabaseAccountsListResult:
    properties:
      value:
        description: This is a default description.
        type: head
  FailoverPolicies:
    properties:
      failoverPolicies:
        description: This is a default description.
        type: head
  FailoverPolicy:
    properties:
      id:
        description: This is a default description.
        type: head
      locationName:
        description: This is a default description.
        type: head
      failoverPriority:
        description: This is a default description.
        type: head
  Location:
    properties:
      id:
        description: This is a default description.
        type: head
      locationName:
        description: This is a default description.
        type: head
      documentEndpoint:
        description: This is a default description.
        type: head
      failoverPriority:
        description: This is a default description.
        type: head
  Resource:
    properties:
      id:
        description: This is a default description.
        type: head
      name:
        description: This is a default description.
        type: head
      type:
        description: This is a default description.
        type: head
      location:
        description: This is a default description.
        type: head
  DatabaseAccount:
    properties:
      kind:
        description: This is a default description.
        type: head
  ConsistencyPolicy:
    properties:
      defaultConsistencyLevel:
        description: This is a default description.
        type: head
      maxStalenessPrefix:
        description: This is a default description.
        type: head
      maxIntervalInSeconds:
        description: This is a default description.
        type: head
  DatabaseAccountProperties:
    properties:
      documentEndpoint:
        description: This is a default description.
        type: head
      writeLocations:
        description: This is a default description.
        type: head
      readLocations:
        description: This is a default description.
        type: head
      failoverPolicies:
        description: This is a default description.
        type: head
  DatabaseAccountCreateUpdateProperties:
    properties:
      locations:
        description: This is a default description.
        type: head
  DatabaseAccountCreateUpdateParameters:
    properties:
      kind:
        description: This is a default description.
        type: head
  DatabaseAccountPatchParameters:
    properties: []
  DatabaseAccountListReadOnlyKeysResult:
    properties:
      primaryReadonlyMasterKey:
        description: This is a default description.
        type: head
      secondaryReadonlyMasterKey:
        description: This is a default description.
        type: head
  DatabaseAccountListKeysResult:
    properties:
      primaryMasterKey:
        description: This is a default description.
        type: head
      secondaryMasterKey:
        description: This is a default description.
        type: head
  DatabaseAccountConnectionString:
    properties:
      connectionString:
        description: This is a default description.
        type: head
      description:
        description: This is a default description.
        type: head
  DatabaseAccountListConnectionStringsResult:
    properties:
      connectionStrings:
        description: This is a default description.
        type: head
  DatabaseAccountRegenerateKeyParameters:
    properties:
      keyKind:
        description: This is a default description.
        type: head
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