---
swagger: "2.0"
info:
  title: Google Play Movies Partner
  description: Gets the delivery status of titles for Google Play Movies Partners.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: playmoviespartner.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/accounts/{accountId}/avails/{availId}:
    get:
      summary: Get Available Movie
      description: Get an Avail given its avail group id and avail id
      operationId: playmoviespartner.accounts.avails.get
      parameters:
      - in: path
        name: accountId
        description: REQUIRED
      - in: path
        name: availId
        description: REQUIRED
      responses:
        200:
          description: OK
      tags:
      - movie
definitions:
  Avail:
    properties:
      altId:
        description: This is a default description.
        type: parameters
      availId:
        description: This is a default description.
        type: parameters
      captionExemption:
        description: This is a default description.
        type: parameters
      captionIncluded:
        description: This is a default description.
        type: parameters
      contentId:
        description: This is a default description.
        type: parameters
      displayName:
        description: This is a default description.
        type: parameters
      encodeId:
        description: This is a default description.
        type: parameters
      end:
        description: This is a default description.
        type: parameters
      episodeAltId:
        description: This is a default description.
        type: parameters
      episodeNumber:
        description: This is a default description.
        type: parameters
  ListAvailsResponse:
    properties:
      avails:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      totalSize:
        description: This is a default description.
        type: parameters
  ListOrdersResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: parameters
      orders:
        description: This is a default description.
        type: parameters
      totalSize:
        description: This is a default description.
        type: parameters
  ListStoreInfosResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: parameters
      storeInfos:
        description: This is a default description.
        type: parameters
      totalSize:
        description: This is a default description.
        type: parameters
  Order:
    properties:
      approvedTime:
        description: This is a default description.
        type: parameters
      channelId:
        description: This is a default description.
        type: parameters
      channelName:
        description: This is a default description.
        type: parameters
      countries:
        description: This is a default description.
        type: parameters
      customId:
        description: This is a default description.
        type: parameters
      earliestAvailStartTime:
        description: This is a default description.
        type: parameters
      episodeName:
        description: This is a default description.
        type: parameters
      legacyPriority:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      normalizedPriority:
        description: This is a default description.
        type: parameters
  StoreInfo:
    properties:
      audioTracks:
        description: This is a default description.
        type: parameters
      country:
        description: This is a default description.
        type: parameters
      editLevelEidr:
        description: This is a default description.
        type: parameters
      episodeNumber:
        description: This is a default description.
        type: parameters
      hasAudio51:
        description: This is a default description.
        type: parameters
      hasEstOffer:
        description: This is a default description.
        type: parameters
      hasHdOffer:
        description: This is a default description.
        type: parameters
      hasInfoCards:
        description: This is a default description.
        type: parameters
      hasSdOffer:
        description: This is a default description.
        type: parameters
      hasVodOffer:
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