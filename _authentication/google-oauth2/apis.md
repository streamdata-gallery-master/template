---
name: Google OAuth2
description: Google APIs use the OAuth 2.0 protocol for authentication and authorization.
  Google supports common OAuth 2.0 scenarios such as those for web server, installed,
  and client-side applications. To begin, obtain OAuth 2.0 client credentials from
  the Google API Console. Then your client application requests an access token from
  the Google Authorization Server, extracts a token from the response, and sends the
  token to the Google API that you want to access. For an interactive demonstration
  of using OAuth 2.0 with Google (including the option to use your own client credentials),
  experiment with the OAuth 2.0 Playground.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-OAuth@2x.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Stack Network
- Security
- Google APIs
- Authentication
created: "2018-02-21"
modified: "2018-02-21"
url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_authentication/google-oauth2/apis.yaml
specificationVersion: "0.14"
apis:
- name: Google OAuth2 APIs
  description: Google APIs use the OAuth 2
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-OAuth@2x.png
  humanURL: https://developers.google.com/identity/protocols/OAuth2
  baseURL: https://developers.google.com/identity/protocols/OAuth2
  tags:
  - Gallery
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_authentication/google-oauth2/oauth2-v2-certs-get.md
- name: Google OAuth2 APIs
  description: Google APIs use the OAuth 2
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-OAuth@2x.png
  humanURL: https://developers.google.com/identity/protocols/OAuth2
  baseURL: https://developers.google.com/identity/protocols/OAuth2
  tags:
  - Gallery
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_authentication/google-oauth2/oauth2-v2-tokeninfo-post.md
- name: Google OAuth2 APIs
  description: Google APIs use the OAuth 2
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-OAuth@2x.png
  humanURL: https://developers.google.com/identity/protocols/OAuth2
  baseURL: https://developers.google.com/identity/protocols/OAuth2
  tags:
  - Gallery
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_authentication/google-oauth2/oauth2-v2-userinfo-get.md
- name: Google OAuth2 APIs
  description: Google APIs use the OAuth 2
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-OAuth@2x.png
  humanURL: https://developers.google.com/identity/protocols/OAuth2
  baseURL: https://developers.google.com/identity/protocols/OAuth2
  tags:
  - Gallery
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_authentication/google-oauth2/userinfo-v2-me-get.md
x-common:
- type: x-website
  url: https://developers.google.com/identity/protocols/OAuth2
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---