---
name: Google People
description: The People API lets you list authenticated users Contacts and retrieve
  profile information for authenticated users and their contacts. For example, lets
  say the authenticated user, Jen, has Fabian and Ranjith in her private contacts.
  When your app calls people.connections.list to retrieve a list of her connections,
  Jen is presented with a consent screen asking to give the app access to the list.
  If Jen consents, the app retrieves a list containing Fabian and Ranjith (with a
  resource name for each person). The app can then call people.get, passing in a resource
  name, to get private contact and public profile data for each person.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-people.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Users
- Stack Network
- People
- Google APIs
created: "2018-02-22"
modified: "2018-02-22"
url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_people/google-people/apis.yaml
specificationVersion: "0.14"
apis:
- name: Google People API
  description: The People API lets you list authenticated users Contacts and retrieve
    profile information for authenticated users and their contacts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-people.png
  humanURL: https://developers.google.com/people/
  baseURL: https://developers.google.com/people/
  tags:
  - Gallery
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_people/google-people/v1-people-batchget-get.md
- name: Google People API
  description: The People API lets you list authenticated users Contacts and retrieve
    profile information for authenticated users and their contacts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-people.png
  humanURL: https://developers.google.com/people/
  baseURL: https://developers.google.com/people/
  tags:
  - Gallery
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_people/google-people/v1-resourcename-get.md
- name: Google People API
  description: The People API lets you list authenticated users Contacts and retrieve
    profile information for authenticated users and their contacts
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-people.png
  humanURL: https://developers.google.com/people/
  baseURL: https://developers.google.com/people/
  tags:
  - Gallery
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_people/google-people/v1-resourcename-connections-get.md
x-common:
- type: x-code-builder
  url: https://developers.google.com/people/v1/libraries
- type: x-terms-of-service-page
  url: https://developers.google.com/people/terms
- type: x-website
  url: https://developers.google.com/people/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---