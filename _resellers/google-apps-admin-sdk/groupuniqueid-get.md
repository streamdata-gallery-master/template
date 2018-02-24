---
swagger: "2.0"
info:
  title: Groups Settings
  description: Lets you manage permission levels and related settings of a group.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /groups/v1/groups
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{groupUniqueId}:
    get:
      summary: Get Group
      description: Gets one resource by id
      operationId: groupsSettings.groups.get
      parameters:
      - in: path
        name: groupUniqueId
        description: The resource ID
      responses:
        200:
          description: OK
      tags:
      - group
definitions:
  Groups:
    properties:
      allowExternalMembers:
        description: This is a default description.
        type: put
      allowGoogleCommunication:
        description: This is a default description.
        type: put
      allowWebPosting:
        description: This is a default description.
        type: put
      archiveOnly:
        description: This is a default description.
        type: put
      customFooterText:
        description: This is a default description.
        type: put
      customReplyTo:
        description: This is a default description.
        type: put
      defaultMessageDenyNotificationText:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      email:
        description: This is a default description.
        type: put
      includeCustomFooter:
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