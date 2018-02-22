---
swagger: "2.0"
info:
  title: Google Drive
  description: Manages files in Drive including uploading, downloading, searching,
    detecting changes, and updating sharing permissions.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /drive/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{fileId}/comments/{commentId}/replies/{replyId}:
    get:
      summary: Get File Comment Reply
      description: Gets a reply by ID
      operationId: drive.replies.get
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: includeDeleted
        description: Whether to return deleted replies
      - in: path
        name: replyId
        description: The ID of the reply
      responses:
        200:
          description: OK
      tags:
      - comment
definitions:
  About:
    properties:
      appInstalled:
        description: This is a default description.
        type: patch
      exportFormats:
        description: This is a default description.
        type: patch
      folderColorPalette:
        description: This is a default description.
        type: patch
      importFormats:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      maxImportSizes:
        description: This is a default description.
        type: patch
      maxUploadSize:
        description: This is a default description.
        type: patch
      storageQuota:
        description: This is a default description.
        type: patch
      canCreateTeamDrives:
        description: This is a default description.
        type: patch
      teamDriveThemes:
        description: This is a default description.
        type: patch
  Change:
    properties:
      fileId:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      removed:
        description: This is a default description.
        type: patch
      teamDriveId:
        description: This is a default description.
        type: patch
      time:
        description: This is a default description.
        type: patch
      type:
        description: This is a default description.
        type: patch
  ChangeList:
    properties:
      changes:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      newStartPageToken:
        description: This is a default description.
        type: patch
      nextPageToken:
        description: This is a default description.
        type: patch
  Channel:
    properties:
      address:
        description: This is a default description.
        type: patch
      expiration:
        description: This is a default description.
        type: patch
      id:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      params:
        description: This is a default description.
        type: patch
      payload:
        description: This is a default description.
        type: patch
      resourceId:
        description: This is a default description.
        type: patch
      resourceUri:
        description: This is a default description.
        type: patch
      token:
        description: This is a default description.
        type: patch
      type:
        description: This is a default description.
        type: patch
  Comment:
    properties:
      anchor:
        description: This is a default description.
        type: patch
      content:
        description: This is a default description.
        type: patch
      createdTime:
        description: This is a default description.
        type: patch
      deleted:
        description: This is a default description.
        type: patch
      htmlContent:
        description: This is a default description.
        type: patch
      id:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      modifiedTime:
        description: This is a default description.
        type: patch
      quotedFileContent:
        description: This is a default description.
        type: patch
      replies:
        description: This is a default description.
        type: patch
  CommentList:
    properties:
      comments:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      nextPageToken:
        description: This is a default description.
        type: patch
  File:
    properties:
      appProperties:
        description: This is a default description.
        type: patch
      capabilities:
        description: This is a default description.
        type: patch
      contentHints:
        description: This is a default description.
        type: patch
      createdTime:
        description: This is a default description.
        type: patch
      description:
        description: This is a default description.
        type: patch
      explicitlyTrashed:
        description: This is a default description.
        type: patch
      fileExtension:
        description: This is a default description.
        type: patch
      folderColorRgb:
        description: This is a default description.
        type: patch
      fullFileExtension:
        description: This is a default description.
        type: patch
      hasAugmentedPermissions:
        description: This is a default description.
        type: patch
  FileList:
    properties:
      files:
        description: This is a default description.
        type: patch
      incompleteSearch:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      nextPageToken:
        description: This is a default description.
        type: patch
  GeneratedIds:
    properties:
      ids:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      space:
        description: This is a default description.
        type: patch
  Permission:
    properties:
      allowFileDiscovery:
        description: This is a default description.
        type: patch
      displayName:
        description: This is a default description.
        type: patch
      domain:
        description: This is a default description.
        type: patch
      emailAddress:
        description: This is a default description.
        type: patch
      expirationTime:
        description: This is a default description.
        type: patch
      id:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      photoLink:
        description: This is a default description.
        type: patch
      role:
        description: This is a default description.
        type: patch
      teamDrivePermissionDetails:
        description: This is a default description.
        type: patch
  PermissionList:
    properties:
      kind:
        description: This is a default description.
        type: patch
      nextPageToken:
        description: This is a default description.
        type: patch
      permissions:
        description: This is a default description.
        type: patch
  Reply:
    properties:
      action:
        description: This is a default description.
        type: patch
      content:
        description: This is a default description.
        type: patch
      createdTime:
        description: This is a default description.
        type: patch
      deleted:
        description: This is a default description.
        type: patch
      htmlContent:
        description: This is a default description.
        type: patch
      id:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      modifiedTime:
        description: This is a default description.
        type: patch
  ReplyList:
    properties:
      kind:
        description: This is a default description.
        type: patch
      nextPageToken:
        description: This is a default description.
        type: patch
      replies:
        description: This is a default description.
        type: patch
  Revision:
    properties:
      id:
        description: This is a default description.
        type: patch
      keepForever:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      md5Checksum:
        description: This is a default description.
        type: patch
      mimeType:
        description: This is a default description.
        type: patch
      modifiedTime:
        description: This is a default description.
        type: patch
      originalFilename:
        description: This is a default description.
        type: patch
      publishAuto:
        description: This is a default description.
        type: patch
      published:
        description: This is a default description.
        type: patch
      publishedOutsideDomain:
        description: This is a default description.
        type: patch
  RevisionList:
    properties:
      kind:
        description: This is a default description.
        type: patch
      nextPageToken:
        description: This is a default description.
        type: patch
      revisions:
        description: This is a default description.
        type: patch
  StartPageToken:
    properties:
      kind:
        description: This is a default description.
        type: patch
      startPageToken:
        description: This is a default description.
        type: patch
  TeamDrive:
    properties:
      capabilities:
        description: This is a default description.
        type: patch
      id:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      name:
        description: This is a default description.
        type: patch
      backgroundImageFile:
        description: This is a default description.
        type: patch
      backgroundImageLink:
        description: This is a default description.
        type: patch
      colorRgb:
        description: This is a default description.
        type: patch
      createdTime:
        description: This is a default description.
        type: patch
      themeId:
        description: This is a default description.
        type: patch
  TeamDriveList:
    properties:
      kind:
        description: This is a default description.
        type: patch
      nextPageToken:
        description: This is a default description.
        type: patch
      teamDrives:
        description: This is a default description.
        type: patch
  User:
    properties:
      displayName:
        description: This is a default description.
        type: patch
      emailAddress:
        description: This is a default description.
        type: patch
      kind:
        description: This is a default description.
        type: patch
      me:
        description: This is a default description.
        type: patch
      permissionId:
        description: This is a default description.
        type: patch
      photoLink:
        description: This is a default description.
        type: patch
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