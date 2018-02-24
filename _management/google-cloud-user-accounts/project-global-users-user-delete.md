---
swagger: "2.0"
info:
  title: Cloud User Accounts
  description: Creates and manages users and groups for accessing Google Compute Engine
    virtual machines.
  contact:
    name: Google
    url: https://google.com
  version: vm_alpha
host: www.googleapis.com
basePath: /clouduseraccounts/vm_alpha/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/users/{user}:
    delete:
      summary: Delete User
      description: Deletes the specified User resource
      operationId: clouduseraccounts.users.delete
      parameters:
      - in: path
        name: project
        description: Project ID for this request
      - in: path
        name: user
        description: Name of the user resource to delete
      responses:
        200:
          description: OK
      tags:
      - user
definitions:
  AuditConfig:
    properties:
      exemptedMembers:
        description: This is a default description.
        type: post
      service:
        description: This is a default description.
        type: post
  AuthorizedKeysView:
    properties:
      keys:
        description: This is a default description.
        type: post
      sudoer:
        description: This is a default description.
        type: post
  Binding:
    properties:
      members:
        description: This is a default description.
        type: post
      role:
        description: This is a default description.
        type: post
  Condition:
    properties:
      iam:
        description: This is a default description.
        type: post
      op:
        description: This is a default description.
        type: post
      svc:
        description: This is a default description.
        type: post
      sys:
        description: This is a default description.
        type: post
      value:
        description: This is a default description.
        type: post
      values:
        description: This is a default description.
        type: post
  Group:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      members:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  GroupList:
    properties:
      id:
        description: This is a default description.
        type: post
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  GroupsAddMemberRequest:
    properties:
      users:
        description: This is a default description.
        type: post
  GroupsRemoveMemberRequest:
    properties:
      users:
        description: This is a default description.
        type: post
  LinuxAccountViews:
    properties:
      groupViews:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      userViews:
        description: This is a default description.
        type: post
  LinuxGetAuthorizedKeysViewResponse:
    properties: []
  LinuxGetLinuxAccountViewsResponse:
    properties: []
  LinuxGroupView:
    properties:
      gid:
        description: This is a default description.
        type: post
      groupName:
        description: This is a default description.
        type: post
      members:
        description: This is a default description.
        type: post
  LinuxUserView:
    properties:
      gecos:
        description: This is a default description.
        type: post
      gid:
        description: This is a default description.
        type: post
      homeDirectory:
        description: This is a default description.
        type: post
      shell:
        description: This is a default description.
        type: post
      uid:
        description: This is a default description.
        type: post
      username:
        description: This is a default description.
        type: post
  LogConfig:
    properties: []
  LogConfigCounterOptions:
    properties:
      field:
        description: This is a default description.
        type: post
      metric:
        description: This is a default description.
        type: post
  Operation:
    properties:
      clientOperationId:
        description: This is a default description.
        type: post
      creationTimestamp:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      endTime:
        description: This is a default description.
        type: post
      error:
        description: This is a default description.
        type: post
      httpErrorMessage:
        description: This is a default description.
        type: post
      httpErrorStatusCode:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      insertTime:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  OperationList:
    properties:
      id:
        description: This is a default description.
        type: post
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  Policy:
    properties:
      auditConfigs:
        description: This is a default description.
        type: post
      bindings:
        description: This is a default description.
        type: post
      etag:
        description: This is a default description.
        type: post
      iamOwned:
        description: This is a default description.
        type: post
      rules:
        description: This is a default description.
        type: post
      version:
        description: This is a default description.
        type: post
  PublicKey:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      expirationTimestamp:
        description: This is a default description.
        type: post
      fingerprint:
        description: This is a default description.
        type: post
      key:
        description: This is a default description.
        type: post
  Rule:
    properties:
      action:
        description: This is a default description.
        type: post
      conditions:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      ins:
        description: This is a default description.
        type: post
      logConfigs:
        description: This is a default description.
        type: post
      notIns:
        description: This is a default description.
        type: post
      permissions:
        description: This is a default description.
        type: post
  TestPermissionsRequest:
    properties:
      permissions:
        description: This is a default description.
        type: post
  TestPermissionsResponse:
    properties:
      permissions:
        description: This is a default description.
        type: post
  User:
    properties:
      creationTimestamp:
        description: This is a default description.
        type: post
      description:
        description: This is a default description.
        type: post
      groups:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
      owner:
        description: This is a default description.
        type: post
      publicKeys:
        description: This is a default description.
        type: post
      selfLink:
        description: This is a default description.
        type: post
  UserList:
    properties:
      id:
        description: This is a default description.
        type: post
      items:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      nextPageToken:
        description: This is a default description.
        type: post
      selfLink:
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