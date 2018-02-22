---
swagger: "2.0"
info:
  title: Search Console
  description: View Google Search Console data for your verified sites.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /webmasters/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sites/{siteUrl}/urlCrawlErrorsCounts/query:
    get:
      summary: Get Crawl Error Count
      description: Retrieves a time series of the number of URL crawl errors per error
        category and platform
      operationId: webmasters.urlcrawlerrorscounts.query
      parameters:
      - in: query
        name: category
        description: The crawl error category
      - in: query
        name: latestCountsOnly
        description: If true, returns only the latest crawl error counts
      - in: query
        name: platform
        description: The user agent type (platform) that made the request
      - in: path
        name: siteUrl
        description: The site's URL, including protocol
      responses:
        200:
          description: OK
      tags:
      - error
definitions:
  ApiDataRow:
    properties:
      clicks:
        description: This is a default description.
        type: parameters
      ctr:
        description: This is a default description.
        type: parameters
      impressions:
        description: This is a default description.
        type: parameters
      keys:
        description: This is a default description.
        type: parameters
      position:
        description: This is a default description.
        type: parameters
  ApiDimensionFilter:
    properties:
      dimension:
        description: This is a default description.
        type: parameters
      expression:
        description: This is a default description.
        type: parameters
      operator:
        description: This is a default description.
        type: parameters
  ApiDimensionFilterGroup:
    properties:
      filters:
        description: This is a default description.
        type: parameters
      groupType:
        description: This is a default description.
        type: parameters
  SearchAnalyticsQueryRequest:
    properties:
      aggregationType:
        description: This is a default description.
        type: parameters
      dimensionFilterGroups:
        description: This is a default description.
        type: parameters
      dimensions:
        description: This is a default description.
        type: parameters
      endDate:
        description: This is a default description.
        type: parameters
      rowLimit:
        description: This is a default description.
        type: parameters
      searchType:
        description: This is a default description.
        type: parameters
      startDate:
        description: This is a default description.
        type: parameters
      startRow:
        description: This is a default description.
        type: parameters
  SearchAnalyticsQueryResponse:
    properties:
      responseAggregationType:
        description: This is a default description.
        type: parameters
      rows:
        description: This is a default description.
        type: parameters
  SitemapsListResponse:
    properties:
      sitemap:
        description: This is a default description.
        type: parameters
  SitesListResponse:
    properties:
      siteEntry:
        description: This is a default description.
        type: parameters
  UrlCrawlErrorCount:
    properties:
      count:
        description: This is a default description.
        type: parameters
      timestamp:
        description: This is a default description.
        type: parameters
  UrlCrawlErrorCountsPerType:
    properties:
      category:
        description: This is a default description.
        type: parameters
      entries:
        description: This is a default description.
        type: parameters
      platform:
        description: This is a default description.
        type: parameters
  UrlCrawlErrorsCountsQueryResponse:
    properties:
      countPerTypes:
        description: This is a default description.
        type: parameters
  UrlCrawlErrorsSample:
    properties:
      first_detected:
        description: This is a default description.
        type: parameters
      last_crawled:
        description: This is a default description.
        type: parameters
      pageUrl:
        description: This is a default description.
        type: parameters
      responseCode:
        description: This is a default description.
        type: parameters
  UrlCrawlErrorsSamplesListResponse:
    properties:
      urlCrawlErrorSample:
        description: This is a default description.
        type: parameters
  UrlSampleDetails:
    properties:
      containingSitemaps:
        description: This is a default description.
        type: parameters
      linkedFromUrls:
        description: This is a default description.
        type: parameters
  WmxSite:
    properties:
      permissionLevel:
        description: This is a default description.
        type: parameters
      siteUrl:
        description: This is a default description.
        type: parameters
  WmxSitemap:
    properties:
      contents:
        description: This is a default description.
        type: parameters
      errors:
        description: This is a default description.
        type: parameters
      isPending:
        description: This is a default description.
        type: parameters
      isSitemapsIndex:
        description: This is a default description.
        type: parameters
      lastDownloaded:
        description: This is a default description.
        type: parameters
      lastSubmitted:
        description: This is a default description.
        type: parameters
      path:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
      warnings:
        description: This is a default description.
        type: parameters
  WmxSitemapContent:
    properties:
      indexed:
        description: This is a default description.
        type: parameters
      submitted:
        description: This is a default description.
        type: parameters
      type:
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