---
name: Google Knowledge Graph Search
description: 'The Knowledge Graph Search API lets you find entities in the Google
  Knowledge Graph. The API uses standard schema.org types and is compliant with the
  JSON-LD specification. Some examples of how you can use the Knowledge Graph Search
  API include: Getting a ranked list of the most notable entities that match certain
  criteria. Predictively completing entities in a search box. Annotating/organizing
  content using the Knowledge Graph entities.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-Knowledge-Graph.jpg
x-kinRank: "9"
x-alexaRank: ""
tags:
- Stack Network
- Search
- Google APIs
created: "2018-02-22"
modified: "2018-02-22"
url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_search/google-knowledge-graph-search/apis.yaml
specificationVersion: "0.14"
apis:
- name: Google Knowledge Graph Search API
  description: The Knowledge Graph Search API lets you find entities in the Google
    Knowledge Graph
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Google-Knowledge-Graph.jpg
  humanURL: https://developers.google.com/knowledge-graph/
  baseURL: https://developers.google.com/knowledge-graph/
  tags:
  - Gallery
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_search/google-knowledge-graph-search/v1-entities-search-get.md
x-common:
- type: x-authentication
  url: https://developers.google.com/knowledge-graph/how-tos/authorizing
- type: x-code-builder
  url: https://developers.google.com/knowledge-graph/libraries
- type: x-rate-limiting
  url: https://developers.google.com/knowledge-graph/reference/rest/v1/usage-limits
- type: x-terms-of-service-page
  url: https://developers.google.com/knowledge-graph/terms
- type: x-website
  url: https://developers.google.com/knowledge-graph/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---