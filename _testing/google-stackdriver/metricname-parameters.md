---
swagger: "2.0"
info:
  title: Google Stackdriver
  description: Writes log entries and manages your Stackdriver Logging configuration.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: logging.googleapis.com
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{metricName}:
    parameters:
      summary: Parameters Metricname
      description: Parameters metricname
      operationId: parametersMetricname
      responses:
        200:
          description: OK
      tags:
      - monitoring
      - metrics
definitions:
  BucketOptions:
    properties: []
  Empty:
    properties: []
  Explicit:
    properties:
      bounds:
        description: This is a default description.
        type: put
  Exponential:
    properties:
      growthFactor:
        description: This is a default description.
        type: put
      numFiniteBuckets:
        description: This is a default description.
        type: put
      scale:
        description: This is a default description.
        type: put
  HttpRequest:
    properties:
      cacheFillBytes:
        description: This is a default description.
        type: put
      cacheHit:
        description: This is a default description.
        type: put
      cacheLookup:
        description: This is a default description.
        type: put
      cacheValidatedWithOriginServer:
        description: This is a default description.
        type: put
      latency:
        description: This is a default description.
        type: put
      protocol:
        description: This is a default description.
        type: put
      referer:
        description: This is a default description.
        type: put
      remoteIp:
        description: This is a default description.
        type: put
      requestMethod:
        description: This is a default description.
        type: put
      requestSize:
        description: This is a default description.
        type: put
  LabelDescriptor:
    properties:
      description:
        description: This is a default description.
        type: put
      key:
        description: This is a default description.
        type: put
      valueType:
        description: This is a default description.
        type: put
  Linear:
    properties:
      numFiniteBuckets:
        description: This is a default description.
        type: put
      offset:
        description: This is a default description.
        type: put
      width:
        description: This is a default description.
        type: put
  ListExclusionsResponse:
    properties:
      exclusions:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  ListLogEntriesRequest:
    properties:
      filter:
        description: This is a default description.
        type: put
      orderBy:
        description: This is a default description.
        type: put
      pageSize:
        description: This is a default description.
        type: put
      pageToken:
        description: This is a default description.
        type: put
      projectIds:
        description: This is a default description.
        type: put
      resourceNames:
        description: This is a default description.
        type: put
  ListLogEntriesResponse:
    properties:
      entries:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  ListLogMetricsResponse:
    properties:
      metrics:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  ListLogsResponse:
    properties:
      logNames:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  ListMonitoredResourceDescriptorsResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: put
      resourceDescriptors:
        description: This is a default description.
        type: put
  ListSinksResponse:
    properties:
      nextPageToken:
        description: This is a default description.
        type: put
      sinks:
        description: This is a default description.
        type: put
  LogEntry:
    properties:
      insertId:
        description: This is a default description.
        type: put
      jsonPayload:
        description: This is a default description.
        type: put
      labels:
        description: This is a default description.
        type: put
      logName:
        description: This is a default description.
        type: put
      protoPayload:
        description: This is a default description.
        type: put
      receiveTimestamp:
        description: This is a default description.
        type: put
      severity:
        description: This is a default description.
        type: put
      spanId:
        description: This is a default description.
        type: put
      textPayload:
        description: This is a default description.
        type: put
      timestamp:
        description: This is a default description.
        type: put
  LogEntryOperation:
    properties:
      first:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      last:
        description: This is a default description.
        type: put
      producer:
        description: This is a default description.
        type: put
  LogEntrySourceLocation:
    properties:
      file:
        description: This is a default description.
        type: put
      function:
        description: This is a default description.
        type: put
      line:
        description: This is a default description.
        type: put
  LogExclusion:
    properties:
      description:
        description: This is a default description.
        type: put
      disabled:
        description: This is a default description.
        type: put
      filter:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
  LogLine:
    properties:
      logMessage:
        description: This is a default description.
        type: put
      severity:
        description: This is a default description.
        type: put
      time:
        description: This is a default description.
        type: put
  LogMetric:
    properties:
      description:
        description: This is a default description.
        type: put
      filter:
        description: This is a default description.
        type: put
      labelExtractors:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      valueExtractor:
        description: This is a default description.
        type: put
      version:
        description: This is a default description.
        type: put
  LogSink:
    properties:
      destination:
        description: This is a default description.
        type: put
      endTime:
        description: This is a default description.
        type: put
      filter:
        description: This is a default description.
        type: put
      includeChildren:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      outputVersionFormat:
        description: This is a default description.
        type: put
      startTime:
        description: This is a default description.
        type: put
      writerIdentity:
        description: This is a default description.
        type: put
  MetricDescriptor:
    properties:
      description:
        description: This is a default description.
        type: put
      displayName:
        description: This is a default description.
        type: put
      labels:
        description: This is a default description.
        type: put
      metricKind:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
      unit:
        description: This is a default description.
        type: put
      valueType:
        description: This is a default description.
        type: put
  MonitoredResource:
    properties:
      labels:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  MonitoredResourceDescriptor:
    properties:
      description:
        description: This is a default description.
        type: put
      displayName:
        description: This is a default description.
        type: put
      labels:
        description: This is a default description.
        type: put
      name:
        description: This is a default description.
        type: put
      type:
        description: This is a default description.
        type: put
  RequestLog:
    properties:
      appEngineRelease:
        description: This is a default description.
        type: put
      appId:
        description: This is a default description.
        type: put
      cost:
        description: This is a default description.
        type: put
      endTime:
        description: This is a default description.
        type: put
      finished:
        description: This is a default description.
        type: put
      first:
        description: This is a default description.
        type: put
      host:
        description: This is a default description.
        type: put
      httpVersion:
        description: This is a default description.
        type: put
      instanceId:
        description: This is a default description.
        type: put
      instanceIndex:
        description: This is a default description.
        type: put
  SourceLocation:
    properties:
      file:
        description: This is a default description.
        type: put
      functionName:
        description: This is a default description.
        type: put
      line:
        description: This is a default description.
        type: put
  SourceReference:
    properties:
      repository:
        description: This is a default description.
        type: put
      revisionId:
        description: This is a default description.
        type: put
  WriteLogEntriesRequest:
    properties:
      dryRun:
        description: This is a default description.
        type: put
      entries:
        description: This is a default description.
        type: put
      labels:
        description: This is a default description.
        type: put
      logName:
        description: This is a default description.
        type: put
      partialSuccess:
        description: This is a default description.
        type: put
  WriteLogEntriesResponse:
    properties: []
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