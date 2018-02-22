---
swagger: "2.0"
info:
  title: Google Civic Information
  description: Provides polling places, early vote locations, contest data, election
    officials, and government representatives for U.S. residential addresses.
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /civicinfo/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /representatives:
    get:
      summary: Lookup Representatives
      description: Looks up political geography and representative information for
        a single address
      operationId: civicinfo.representatives.representativeInfoByAddress
      parameters:
      - in: query
        name: address
        description: The address to look up
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: includeOffices
        description: Whether to return information about offices and officials
      - in: query
        name: levels
        description: A list of office levels to filter by
      - in: query
        name: roles
        description: A list of office roles to filter by
      responses:
        200:
          description: OK
      tags:
      - representative
definitions:
  AdministrationRegion:
    properties:
      id:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      sources:
        description: This is a default description.
        type: parameters
  AdministrativeBody:
    properties:
      absenteeVotingInfoUrl:
        description: This is a default description.
        type: parameters
      addressLines:
        description: This is a default description.
        type: parameters
      ballotInfoUrl:
        description: This is a default description.
        type: parameters
      electionInfoUrl:
        description: This is a default description.
        type: parameters
      electionOfficials:
        description: This is a default description.
        type: parameters
      electionRegistrationConfirmationUrl:
        description: This is a default description.
        type: parameters
      electionRegistrationUrl:
        description: This is a default description.
        type: parameters
      electionRulesUrl:
        description: This is a default description.
        type: parameters
      hoursOfOperation:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
  Candidate:
    properties:
      candidateUrl:
        description: This is a default description.
        type: parameters
      channels:
        description: This is a default description.
        type: parameters
      email:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      orderOnBallot:
        description: This is a default description.
        type: parameters
      party:
        description: This is a default description.
        type: parameters
      phone:
        description: This is a default description.
        type: parameters
      photoUrl:
        description: This is a default description.
        type: parameters
  Channel:
    properties:
      id:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  Contest:
    properties:
      ballotPlacement:
        description: This is a default description.
        type: parameters
      candidates:
        description: This is a default description.
        type: parameters
      electorateSpecifications:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      level:
        description: This is a default description.
        type: parameters
      numberElected:
        description: This is a default description.
        type: parameters
      numberVotingFor:
        description: This is a default description.
        type: parameters
      office:
        description: This is a default description.
        type: parameters
      primaryParty:
        description: This is a default description.
        type: parameters
      referendumBallotResponses:
        description: This is a default description.
        type: parameters
  ContextParams:
    properties:
      clientProfile:
        description: This is a default description.
        type: parameters
  DivisionRepresentativeInfoRequest:
    properties: []
  DivisionSearchRequest:
    properties: []
  DivisionSearchResponse:
    properties:
      kind:
        description: This is a default description.
        type: parameters
      results:
        description: This is a default description.
        type: parameters
  DivisionSearchResult:
    properties:
      aliases:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      ocdId:
        description: This is a default description.
        type: parameters
  Election:
    properties:
      electionDay:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      ocdDivisionId:
        description: This is a default description.
        type: parameters
  ElectionOfficial:
    properties:
      emailAddress:
        description: This is a default description.
        type: parameters
      faxNumber:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      officePhoneNumber:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
  ElectionsQueryRequest:
    properties: []
  ElectionsQueryResponse:
    properties:
      elections:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  ElectoralDistrict:
    properties:
      id:
        description: This is a default description.
        type: parameters
      kgForeignKey:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      scope:
        description: This is a default description.
        type: parameters
  GeographicDivision:
    properties:
      alsoKnownAs:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      officeIndices:
        description: This is a default description.
        type: parameters
  Office:
    properties:
      divisionId:
        description: This is a default description.
        type: parameters
      levels:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      officialIndices:
        description: This is a default description.
        type: parameters
      roles:
        description: This is a default description.
        type: parameters
      sources:
        description: This is a default description.
        type: parameters
  Official:
    properties:
      address:
        description: This is a default description.
        type: parameters
      channels:
        description: This is a default description.
        type: parameters
      emails:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      party:
        description: This is a default description.
        type: parameters
      phones:
        description: This is a default description.
        type: parameters
      photoUrl:
        description: This is a default description.
        type: parameters
      urls:
        description: This is a default description.
        type: parameters
  PollingLocation:
    properties:
      endDate:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      name:
        description: This is a default description.
        type: parameters
      notes:
        description: This is a default description.
        type: parameters
      pollingHours:
        description: This is a default description.
        type: parameters
      sources:
        description: This is a default description.
        type: parameters
      startDate:
        description: This is a default description.
        type: parameters
      voterServices:
        description: This is a default description.
        type: parameters
  PostalAddress:
    properties:
      addressLines:
        description: This is a default description.
        type: parameters
      administrativeAreaName:
        description: This is a default description.
        type: parameters
      countryName:
        description: This is a default description.
        type: parameters
      countryNameCode:
        description: This is a default description.
        type: parameters
      dependentLocalityName:
        description: This is a default description.
        type: parameters
      dependentThoroughfareLeadingType:
        description: This is a default description.
        type: parameters
      dependentThoroughfareName:
        description: This is a default description.
        type: parameters
      dependentThoroughfarePostDirection:
        description: This is a default description.
        type: parameters
      dependentThoroughfarePreDirection:
        description: This is a default description.
        type: parameters
      dependentThoroughfareTrailingType:
        description: This is a default description.
        type: parameters
  RepresentativeInfoData:
    properties:
      divisions:
        description: This is a default description.
        type: parameters
      offices:
        description: This is a default description.
        type: parameters
      officials:
        description: This is a default description.
        type: parameters
  RepresentativeInfoRequest:
    properties: []
  RepresentativeInfoResponse:
    properties:
      divisions:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      offices:
        description: This is a default description.
        type: parameters
      officials:
        description: This is a default description.
        type: parameters
  SimpleAddressType:
    properties:
      city:
        description: This is a default description.
        type: parameters
      line1:
        description: This is a default description.
        type: parameters
      line2:
        description: This is a default description.
        type: parameters
      line3:
        description: This is a default description.
        type: parameters
      locationName:
        description: This is a default description.
        type: parameters
      state:
        description: This is a default description.
        type: parameters
      zip:
        description: This is a default description.
        type: parameters
  Source:
    properties:
      name:
        description: This is a default description.
        type: parameters
      official:
        description: This is a default description.
        type: parameters
  VoterInfoRequest:
    properties: []
  VoterInfoResponse:
    properties:
      contests:
        description: This is a default description.
        type: parameters
      dropOffLocations:
        description: This is a default description.
        type: parameters
      earlyVoteSites:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      mailOnly:
        description: This is a default description.
        type: parameters
      otherElections:
        description: This is a default description.
        type: parameters
      pollingLocations:
        description: This is a default description.
        type: parameters
      precinctId:
        description: This is a default description.
        type: parameters
      state:
        description: This is a default description.
        type: parameters
  VoterInfoSegmentResult:
    properties:
      generatedMillis:
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