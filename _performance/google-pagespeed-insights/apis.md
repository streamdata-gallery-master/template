---
name: Google PageSpeed Insights
description: Page Speed Insights measures the performance of a page for mobile devices
  and desktop devices. It fetches the url twice, once with a mobile user-agent, and
  once with a desktop-user agent. The PageSpeed Score ranges from 0 to 100 points.
  A higher score is better and a score of 85 or above indicates that the page is performing
  well. Please note that PageSpeed Insights is being continually improved and so the
  score will change as we add new rules or improve our analysis.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/54de5c09d56ec853cc9310e1.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Websites
- Stack Network
- Performance
- Google APIs
created: "2018-02-22"
modified: "2018-02-22"
url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_performance/google-pagespeed-insights/apis.yaml
specificationVersion: "0.14"
apis:
- name: Google PageSpeed Insights API
  description: Page Speed Insights measures the performance of a page for mobile devices
    and desktop devices
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/54de5c09d56ec853cc9310e1.png
  humanURL: https://developers.google.com/speed/docs/insights/about
  baseURL: https://developers.google.com/speed/docs/insights/about
  tags:
  - Gallery
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery/apis/master/_performance/google-pagespeed-insights/runpagespeed-get.md
x-common:
- type: x-change-logs
  url: https://developers.google.com/speed/docs/insights/release_notes
- type: x-getting-started
  url: https://developers.google.com/speed/docs/insights/v2/getting-started
- type: x-website
  url: https://developers.google.com/speed/docs/insights/about
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---