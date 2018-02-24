---
swagger: "2.0"
info:
  title: Google Play Developer
  description: Lets Android application developers access their Google Play accounts.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /androidpublisher/v2/applications
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{packageName}/reviews/{reviewId}:
    get:
      summary: Get Review
      description: Returns a single review
      operationId: androidpublisher.reviews.get
      parameters:
      - in: path
        name: packageName
        description: Unique identifier for the Android app for which we want reviews;
          for example, "com
      - in: path
        name: reviewId
      - in: query
        name: translationLanguage
      responses:
        200:
          description: OK
      tags:
      - review
definitions:
  Apk:
    properties:
      versionCode:
        description: This is a default description.
        type: post
  ApkBinary:
    properties:
      sha1:
        description: This is a default description.
        type: post
  ApkListing:
    properties:
      language:
        description: This is a default description.
        type: post
      recentChanges:
        description: This is a default description.
        type: post
  ApkListingsListResponse:
    properties:
      kind:
        description: This is a default description.
        type: post
      listings:
        description: This is a default description.
        type: post
  ApksAddExternallyHostedRequest:
    properties: []
  ApksAddExternallyHostedResponse:
    properties: []
  ApksListResponse:
    properties:
      apks:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  AppDetails:
    properties:
      contactEmail:
        description: This is a default description.
        type: post
      contactPhone:
        description: This is a default description.
        type: post
      contactWebsite:
        description: This is a default description.
        type: post
      defaultLanguage:
        description: This is a default description.
        type: post
  AppEdit:
    properties:
      expiryTimeSeconds:
        description: This is a default description.
        type: post
      id:
        description: This is a default description.
        type: post
  Comment:
    properties: []
  DeobfuscationFile:
    properties:
      symbolType:
        description: This is a default description.
        type: post
  DeobfuscationFilesUploadResponse:
    properties: []
  DeveloperComment:
    properties:
      text:
        description: This is a default description.
        type: post
  DeviceMetadata:
    properties:
      cpuMake:
        description: This is a default description.
        type: post
      cpuModel:
        description: This is a default description.
        type: post
      deviceClass:
        description: This is a default description.
        type: post
      glEsVersion:
        description: This is a default description.
        type: post
      manufacturer:
        description: This is a default description.
        type: post
      nativePlatform:
        description: This is a default description.
        type: post
      productName:
        description: This is a default description.
        type: post
      ramMb:
        description: This is a default description.
        type: post
      screenDensityDpi:
        description: This is a default description.
        type: post
      screenHeightPx:
        description: This is a default description.
        type: post
  Entitlement:
    properties:
      kind:
        description: This is a default description.
        type: post
      productId:
        description: This is a default description.
        type: post
      productType:
        description: This is a default description.
        type: post
      token:
        description: This is a default description.
        type: post
  EntitlementsListResponse:
    properties:
      resources:
        description: This is a default description.
        type: post
  ExpansionFile:
    properties:
      fileSize:
        description: This is a default description.
        type: post
      referencesVersion:
        description: This is a default description.
        type: post
  ExpansionFilesUploadResponse:
    properties: []
  ExternallyHostedApk:
    properties:
      applicationLabel:
        description: This is a default description.
        type: post
      certificateBase64s:
        description: This is a default description.
        type: post
      externallyHostedUrl:
        description: This is a default description.
        type: post
      fileSha1Base64:
        description: This is a default description.
        type: post
      fileSha256Base64:
        description: This is a default description.
        type: post
      fileSize:
        description: This is a default description.
        type: post
      iconBase64:
        description: This is a default description.
        type: post
      maximumSdk:
        description: This is a default description.
        type: post
      minimumSdk:
        description: This is a default description.
        type: post
      nativeCodes:
        description: This is a default description.
        type: post
  ExternallyHostedApkUsesPermission:
    properties:
      maxSdkVersion:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  Image:
    properties:
      id:
        description: This is a default description.
        type: post
      sha1:
        description: This is a default description.
        type: post
      url:
        description: This is a default description.
        type: post
  ImagesDeleteAllResponse:
    properties:
      deleted:
        description: This is a default description.
        type: post
  ImagesListResponse:
    properties:
      images:
        description: This is a default description.
        type: post
  ImagesUploadResponse:
    properties: []
  InAppProduct:
    properties:
      defaultLanguage:
        description: This is a default description.
        type: post
      listings:
        description: This is a default description.
        type: post
      packageName:
        description: This is a default description.
        type: post
      prices:
        description: This is a default description.
        type: post
      purchaseType:
        description: This is a default description.
        type: post
      sku:
        description: This is a default description.
        type: post
      status:
        description: This is a default description.
        type: post
      subscriptionPeriod:
        description: This is a default description.
        type: post
      trialPeriod:
        description: This is a default description.
        type: post
  InAppProductListing:
    properties:
      description:
        description: This is a default description.
        type: post
      title:
        description: This is a default description.
        type: post
  InappproductsBatchRequest:
    properties:
      entrys:
        description: This is a default description.
        type: post
  InappproductsBatchRequestEntry:
    properties:
      batchId:
        description: This is a default description.
        type: post
      methodName:
        description: This is a default description.
        type: post
  InappproductsBatchResponse:
    properties:
      entrys:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  InappproductsBatchResponseEntry:
    properties:
      batchId:
        description: This is a default description.
        type: post
  InappproductsInsertRequest:
    properties: []
  InappproductsInsertResponse:
    properties: []
  InappproductsListResponse:
    properties:
      inappproduct:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
  InappproductsUpdateRequest:
    properties: []
  InappproductsUpdateResponse:
    properties: []
  Listing:
    properties:
      fullDescription:
        description: This is a default description.
        type: post
      language:
        description: This is a default description.
        type: post
      shortDescription:
        description: This is a default description.
        type: post
      title:
        description: This is a default description.
        type: post
      video:
        description: This is a default description.
        type: post
  ListingsListResponse:
    properties:
      kind:
        description: This is a default description.
        type: post
      listings:
        description: This is a default description.
        type: post
  MonthDay:
    properties:
      day:
        description: This is a default description.
        type: post
      month:
        description: This is a default description.
        type: post
  PageInfo:
    properties:
      resultPerPage:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      totalResults:
        description: This is a default description.
        type: post
  Price:
    properties:
      currency:
        description: This is a default description.
        type: post
      priceMicros:
        description: This is a default description.
        type: post
  ProductPurchase:
    properties:
      consumptionState:
        description: This is a default description.
        type: post
      developerPayload:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      purchaseState:
        description: This is a default description.
        type: post
      purchaseTimeMillis:
        description: This is a default description.
        type: post
  Prorate:
    properties: []
  Review:
    properties:
      authorName:
        description: This is a default description.
        type: post
      comments:
        description: This is a default description.
        type: post
      reviewId:
        description: This is a default description.
        type: post
  ReviewReplyResult:
    properties:
      replyText:
        description: This is a default description.
        type: post
  ReviewsListResponse:
    properties:
      reviews:
        description: This is a default description.
        type: post
  ReviewsReplyRequest:
    properties:
      replyText:
        description: This is a default description.
        type: post
  ReviewsReplyResponse:
    properties: []
  Season:
    properties:
      prorations:
        description: This is a default description.
        type: post
  SubscriptionDeferralInfo:
    properties:
      desiredExpiryTimeMillis:
        description: This is a default description.
        type: post
      expectedExpiryTimeMillis:
        description: This is a default description.
        type: post
  SubscriptionPurchase:
    properties:
      autoRenewing:
        description: This is a default description.
        type: post
      cancelReason:
        description: This is a default description.
        type: post
      countryCode:
        description: This is a default description.
        type: post
      developerPayload:
        description: This is a default description.
        type: post
      expiryTimeMillis:
        description: This is a default description.
        type: post
      kind:
        description: This is a default description.
        type: post
      paymentState:
        description: This is a default description.
        type: post
      priceAmountMicros:
        description: This is a default description.
        type: post
      priceCurrencyCode:
        description: This is a default description.
        type: post
      startTimeMillis:
        description: This is a default description.
        type: post
  SubscriptionPurchasesDeferRequest:
    properties: []
  SubscriptionPurchasesDeferResponse:
    properties:
      newExpiryTimeMillis:
        description: This is a default description.
        type: post
  Testers:
    properties:
      googleGroups:
        description: This is a default description.
        type: post
      googlePlusCommunities:
        description: This is a default description.
        type: post
  Timestamp:
    properties:
      nanos:
        description: This is a default description.
        type: post
      seconds:
        description: This is a default description.
        type: post
  TokenPagination:
    properties:
      nextPageToken:
        description: This is a default description.
        type: post
      previousPageToken:
        description: This is a default description.
        type: post
  Track:
    properties:
      track:
        description: This is a default description.
        type: post
      userFraction:
        description: This is a default description.
        type: post
      versionCodes:
        description: This is a default description.
        type: post
  TracksListResponse:
    properties:
      kind:
        description: This is a default description.
        type: post
      tracks:
        description: This is a default description.
        type: post
  UserComment:
    properties:
      androidOsVersion:
        description: This is a default description.
        type: post
      appVersionCode:
        description: This is a default description.
        type: post
      appVersionName:
        description: This is a default description.
        type: post
      device:
        description: This is a default description.
        type: post
      originalText:
        description: This is a default description.
        type: post
      reviewerLanguage:
        description: This is a default description.
        type: post
      starRating:
        description: This is a default description.
        type: post
      text:
        description: This is a default description.
        type: post
      thumbsDownCount:
        description: This is a default description.
        type: post
      thumbsUpCount:
        description: This is a default description.
        type: post
  VoidedPurchase:
    properties:
      kind:
        description: This is a default description.
        type: post
      purchaseTimeMillis:
        description: This is a default description.
        type: post
      purchaseToken:
        description: This is a default description.
        type: post
      voidedTimeMillis:
        description: This is a default description.
        type: post
  VoidedPurchasesListResponse:
    properties:
      voidedPurchases:
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