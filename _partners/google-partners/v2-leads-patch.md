---
swagger: "2.0"
info:
  title: Google Partners
  description: Searches certified companies and creates contact leads with them, and
    also audits the usage of clients.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: partners.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/leads:
    patch:
      summary: Update Lead
      description: Updates the specified lead
      operationId: partners.updateLeads
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: requestMetadata.experimentIds
        description: Experiment IDs the current request belongs to
      - in: query
        name: requestMetadata.locale
        description: Locale to use for the current request
      - in: query
        name: requestMetadata.partnersSessionId
        description: Google Partners session ID
      - in: query
        name: requestMetadata.trafficSource.trafficSourceId
        description: Identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.trafficSource.trafficSubId
        description: Second level identifier to indicate where the traffic comes from
      - in: query
        name: requestMetadata.userOverrides.ipAddress
        description: IP address to use instead of the user's geo-located IP address
      - in: query
        name: requestMetadata.userOverrides.userId
        description: Logged-in user ID to impersonate instead of the user's ID
      - in: query
        name: updateMask
        description: Standard field mask for the set of fields to be updated
      responses:
        200:
          description: OK
      tags:
      - lead
definitions:
  AdWordsManagerAccountInfo:
    properties:
      customerName:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
  Analytics:
    properties: []
  AnalyticsDataPoint:
    properties:
      eventCount:
        description: This is a default description.
        type: put
      eventLocations:
        description: This is a default description.
        type: put
  AnalyticsSummary:
    properties:
      contactsCount:
        description: This is a default description.
        type: put
      profileViewsCount:
        description: This is a default description.
        type: put
      searchViewsCount:
        description: This is a default description.
        type: put
  AvailableOffer:
    properties:
      available:
        description: This is a default description.
        type: put
      countryOfferInfos:
        description: This is a default description.
        type: put
      description:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      maxAccountAge:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      offerLevel:
        description: This is a default description.
        type: put
      offerType:
        description: This is a default description.
        type: put
      qualifiedCustomer:
        description: This is a default description.
        type: put
      qualifiedCustomersComplete:
        description: This is a default description.
        type: put
  Certification:
    properties:
      achieved:
        description: This is a default description.
        type: put
      certificationType:
        description: This is a default description.
        type: put
      expiration:
        description: This is a default description.
        type: put
      lastAchieved:
        description: This is a default description.
        type: put
      warning:
        description: This is a default description.
        type: put
  CertificationExamStatus:
    properties:
      numberUsersPass:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  CertificationStatus:
    properties:
      examStatuses:
        description: This is a default description.
        type: put
      isCertified:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      userCount:
        description: This is a default description.
        type: put
  Company:
    properties:
      additionalWebsites:
        description: This is a default description.
        type: put
      autoApprovalEmailDomains:
        description: This is a default description.
        type: put
      badgeTier:
        description: This is a default description.
        type: put
      certificationStatuses:
        description: This is a default description.
        type: put
      companyTypes:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      industries:
        description: This is a default description.
        type: put
      localizedInfos:
        description: This is a default description.
        type: put
      locations:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
  CompanyRelation:
    properties:
      address:
        description: This is a default description.
        type: put
      badgeTier:
        description: This is a default description.
        type: put
      companyAdmin:
        description: This is a default description.
        type: put
      companyId:
        description: This is a default description.
        type: put
      creationTime:
        description: This is a default description.
        type: put
      isPending:
        description: This is a default description.
        type: put
      logoUrl:
        description: This is a default description.
        type: put
      managerAccount:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      phoneNumber:
        description: This is a default description.
        type: put
  CountryOfferInfo:
    properties:
      getYAmount:
        description: This is a default description.
        type: put
      offerCountryCode:
        description: This is a default description.
        type: put
      offerType:
        description: This is a default description.
        type: put
      spendXAmount:
        description: This is a default description.
        type: put
  CreateLeadRequest:
    properties: []
  CreateLeadResponse:
    properties:
      recaptchaStatus:
        description: This is a default description.
        type: put
  Date:
    properties:
      day:
        description: This is a default description.
        type: put
      month:
        description: This is a default description.
        type: put
      year:
        description: This is a default description.
        type: put
  DebugInfo:
    properties:
      serverInfo:
        description: This is a default description.
        type: put
      serverTraceInfo:
        description: This is a default description.
        type: put
      serviceUrl:
        description: This is a default description.
        type: put
  Empty:
    properties: []
  EventData:
    properties:
      key:
        description: This is a default description.
        type: put
      values:
        description: This is a default description.
        type: put
  ExamStatus:
    properties:
      examType:
        description: This is a default description.
        type: put
      expiration:
        description: This is a default description.
        type: put
      lastPassed:
        description: This is a default description.
        type: put
      passed:
        description: This is a default description.
        type: put
      taken:
        description: This is a default description.
        type: put
      warning:
        description: This is a default description.
        type: put
  ExamToken:
    properties:
      examId:
        description: This is a default description.
        type: put
      examType:
        description: This is a default description.
        type: put
      token:
        description: This is a default description.
        type: put
  GetCompanyResponse:
    properties: []
  GetPartnersStatusResponse:
    properties: []
  HistoricalOffer:
    properties:
      adwordsUrl:
        description: This is a default description.
        type: put
      clientEmail:
        description: This is a default description.
        type: put
      clientId:
        description: This is a default description.
        type: put
      clientName:
        description: This is a default description.
        type: put
      creationTime:
        description: This is a default description.
        type: put
      expirationTime:
        description: This is a default description.
        type: put
      lastModifiedTime:
        description: This is a default description.
        type: put
      offerCode:
        description: This is a default description.
        type: put
      offerCountryCode:
        description: This is a default description.
        type: put
      offerType:
        description: This is a default description.
        type: put
  LatLng:
    properties:
      latitude:
        description: This is a default description.
        type: put
      longitude:
        description: This is a default description.
        type: put
  Lead:
    properties:
      adwordsCustomerId:
        description: This is a default description.
        type: put
      comments:
        description: This is a default description.
        type: put
      createTime:
        description: This is a default description.
        type: put
      email:
        description: This is a default description.
        type: put
      familyName:
        description: This is a default description.
        type: put
      givenName:
        description: This is a default description.
        type: put
      gpsMotivations:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      languageCode:
        description: This is a default description.
        type: put
      marketingOptIn:
        description: This is a default description.
        type: put
  ListAnalyticsResponse:
    properties:
      analytics:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  ListCompaniesResponse:
    properties:
      companies:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  ListLeadsResponse:
    properties:
      leads:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
      totalSize:
        description: This is a default description.
        type: put
  ListOffersHistoryResponse:
    properties:
      canShowEntireCompany:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
      offers:
        description: This is a default description.
        type: put
      showingEntireCompany:
        description: This is a default description.
        type: put
      totalResults:
        description: This is a default description.
        type: put
  ListOffersResponse:
    properties:
      availableOffers:
        description: This is a default description.
        type: put
      noOfferReason:
        description: This is a default description.
        type: put
  ListUserStatesResponse:
    properties:
      userStates:
        description: This is a default description.
        type: put
  LocalizedCompanyInfo:
    properties:
      countryCodes:
        description: This is a default description.
        type: put
      displayName:
        description: This is a default description.
        type: put
      languageCode:
        description: This is a default description.
        type: put
      overview:
        description: This is a default description.
        type: put
  Location:
    properties:
      address:
        description: This is a default description.
        type: put
      addressLine:
        description: This is a default description.
        type: put
      administrativeArea:
        description: This is a default description.
        type: put
      dependentLocality:
        description: This is a default description.
        type: put
      languageCode:
        description: This is a default description.
        type: put
      locality:
        description: This is a default description.
        type: put
      postalCode:
        description: This is a default description.
        type: put
      regionCode:
        description: This is a default description.
        type: put
      sortingCode:
        description: This is a default description.
        type: put
  LogMessageRequest:
    properties:
      clientInfo:
        description: This is a default description.
        type: put
      details:
        description: This is a default description.
        type: put
      level:
        description: This is a default description.
        type: put
  LogMessageResponse:
    properties: []
  LogUserEventRequest:
    properties:
      eventAction:
        description: This is a default description.
        type: put
      eventCategory:
        description: This is a default description.
        type: put
      eventDatas:
        description: This is a default description.
        type: put
      eventScope:
        description: This is a default description.
        type: put
      url:
        description: This is a default description.
        type: put
  LogUserEventResponse:
    properties: []
  Money:
    properties:
      currencyCode:
        description: This is a default description.
        type: put
      nanos:
        description: This is a default description.
        type: put
      units:
        description: This is a default description.
        type: put
  OfferCustomer:
    properties:
      adwordsUrl:
        description: This is a default description.
        type: put
      countryCode:
        description: This is a default description.
        type: put
      creationTime:
        description: This is a default description.
        type: put
      eligibilityDaysLeft:
        description: This is a default description.
        type: put
      externalCid:
        description: This is a default description.
        type: put
      getYAmount:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      offerType:
        description: This is a default description.
        type: put
      spendXAmount:
        description: This is a default description.
        type: put
  OptIns:
    properties:
      marketComm:
        description: This is a default description.
        type: put
      performanceSuggestions:
        description: This is a default description.
        type: put
      phoneContact:
        description: This is a default description.
        type: put
      physicalMail:
        description: This is a default description.
        type: put
      specialOffers:
        description: This is a default description.
        type: put
  PublicProfile:
    properties:
      displayImageUrl:
        description: This is a default description.
        type: put
      displayName:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      profileImage:
        description: This is a default description.
        type: put
      url:
        description: This is a default description.
        type: put
  Rank:
    properties:
      type:
        description: This is a default description.
        type: put
      value:
        description: This is a default description.
        type: put
  RecaptchaChallenge:
    properties:
      id:
        description: This is a default description.
        type: put
      response:
        description: This is a default description.
        type: put
  RequestMetadata:
    properties:
      experimentIds:
        description: This is a default description.
        type: put
      locale:
        description: This is a default description.
        type: put
      partnersSessionId:
        description: This is a default description.
        type: put
  ResponseMetadata:
    properties: []
  SpecializationStatus:
    properties:
      badgeSpecialization:
        description: This is a default description.
        type: put
      badgeSpecializationState:
        description: This is a default description.
        type: put
  TrafficSource:
    properties:
      trafficSourceId:
        description: This is a default description.
        type: put
      trafficSubId:
        description: This is a default description.
        type: put
  User:
    properties:
      availableAdwordsManagerAccounts:
        description: This is a default description.
        type: put
      certificationStatus:
        description: This is a default description.
        type: put
      companyVerificationEmail:
        description: This is a default description.
        type: put
      examStatus:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      lastAccessTime:
        description: This is a default description.
        type: put
      primaryEmails:
        description: This is a default description.
        type: put
  UserOverrides:
    properties:
      ipAddress:
        description: This is a default description.
        type: put
      userId:
        description: This is a default description.
        type: put
  UserProfile:
    properties:
      adwordsManagerAccount:
        description: This is a default description.
        type: put
      channels:
        description: This is a default description.
        type: put
      emailAddress:
        description: This is a default description.
        type: put
      familyName:
        description: This is a default description.
        type: put
      givenName:
        description: This is a default description.
        type: put
      industries:
        description: This is a default description.
        type: put
      jobFunctions:
        description: This is a default description.
        type: put
      languages:
        description: This is a default description.
        type: put
      markets:
        description: This is a default description.
        type: put
      phoneNumber:
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