---
swagger: "2.0"
info:
  title: Google Calendar
  description: Manipulates events and other calendar data.
  contact:
    name: Google
    url: https://google.com
  version: v3/
host: www.googleapis.com
basePath: /calendar/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calendars/{calendarId}/events/watch:
    post:
      summary: Watch Event
      description: Watch for changes to Events resources
      operationId: calendar.events.watch
      parameters:
      - in: query
        name: alwaysIncludeEmail
        description: Whether to always include a value in the email field for the
          organizer, creator and attendees, even if no real email is available (i
      - in: path
        name: calendarId
        description: Calendar identifier
      - in: query
        name: iCalUID
        description: Specifies event ID in the iCalendar format to be included in
          the response
      - in: query
        name: maxAttendees
        description: The maximum number of attendees to include in the response
      - in: query
        name: maxResults
        description: Maximum number of events returned on one result page
      - in: query
        name: orderBy
        description: The order of the events returned in the result
      - in: query
        name: pageToken
        description: Token specifying which result page to return
      - in: query
        name: privateExtendedProperty
        description: Extended properties constraint specified as propertyName=value
      - in: query
        name: q
        description: Free text search terms to find events that match these terms
          in any field, except for extended properties
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: sharedExtendedProperty
        description: Extended properties constraint specified as propertyName=value
      - in: query
        name: showDeleted
        description: Whether to include deleted events (with status equals "cancelled")
          in the result
      - in: query
        name: showHiddenInvitations
        description: Whether to include hidden invitations in the result
      - in: query
        name: singleEvents
        description: Whether to expand recurring events into instances and only return
          single one-off events and instances of recurring events, but not the underlying
          recurring events themselves
      - in: query
        name: syncToken
        description: Token obtained from the nextSyncToken field returned on the last
          page of results from the previous list request
      - in: query
        name: timeMax
        description: Upper bound (exclusive) for an event's start time to filter by
      - in: query
        name: timeMin
        description: Lower bound (inclusive) for an event's end time to filter by
      - in: query
        name: timeZone
        description: Time zone used in the response
      - in: query
        name: updatedMin
        description: Lower bound for an event's last modification time (as a RFC3339
          timestamp) to filter by
      responses:
        200:
          description: OK
      tags:
      - event
definitions:
  Acl:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      nextSyncToken:
        description: This is a default description.
        type: parameters
  AclRule:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      role:
        description: This is a default description.
        type: parameters
      scope:
        description: This is a default description.
        type: parameters
  Calendar:
    properties:
      description:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      location:
        description: This is a default description.
        type: parameters
      summary:
        description: This is a default description.
        type: parameters
      timeZone:
        description: This is a default description.
        type: parameters
  CalendarList:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      nextSyncToken:
        description: This is a default description.
        type: parameters
  CalendarListEntry:
    properties:
      accessRole:
        description: This is a default description.
        type: parameters
      backgroundColor:
        description: This is a default description.
        type: parameters
      colorId:
        description: This is a default description.
        type: parameters
      defaultReminders:
        description: This is a default description.
        type: parameters
      deleted:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      foregroundColor:
        description: This is a default description.
        type: parameters
      hidden:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
  CalendarNotification:
    properties:
      method:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  Channel:
    properties:
      address:
        description: This is a default description.
        type: parameters
      expiration:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      params:
        description: This is a default description.
        type: parameters
      payload:
        description: This is a default description.
        type: parameters
      resourceId:
        description: This is a default description.
        type: parameters
      resourceUri:
        description: This is a default description.
        type: parameters
      token:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  ColorDefinition:
    properties:
      background:
        description: This is a default description.
        type: parameters
      foreground:
        description: This is a default description.
        type: parameters
  Colors:
    properties:
      calendar:
        description: This is a default description.
        type: parameters
      event:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      updated:
        description: This is a default description.
        type: parameters
  Error:
    properties:
      domain:
        description: This is a default description.
        type: parameters
      reason:
        description: This is a default description.
        type: parameters
  Event:
    properties:
      anyoneCanAddSelf:
        description: This is a default description.
        type: parameters
      attachments:
        description: This is a default description.
        type: parameters
      attendees:
        description: This is a default description.
        type: parameters
      attendeesOmitted:
        description: This is a default description.
        type: parameters
      colorId:
        description: This is a default description.
        type: parameters
      created:
        description: This is a default description.
        type: parameters
      creator:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      endTimeUnspecified:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
  EventAttachment:
    properties:
      fileId:
        description: This is a default description.
        type: parameters
      fileUrl:
        description: This is a default description.
        type: parameters
      iconLink:
        description: This is a default description.
        type: parameters
      mimeType:
        description: This is a default description.
        type: parameters
      title:
        description: This is a default description.
        type: parameters
  EventAttendee:
    properties:
      additionalGuests:
        description: This is a default description.
        type: parameters
      comment:
        description: This is a default description.
        type: parameters
      displayName:
        description: This is a default description.
        type: parameters
      email:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      optional:
        description: This is a default description.
        type: parameters
      organizer:
        description: This is a default description.
        type: parameters
      resource:
        description: This is a default description.
        type: parameters
      responseStatus:
        description: This is a default description.
        type: parameters
      self:
        description: This is a default description.
        type: parameters
  EventDateTime:
    properties:
      date:
        description: This is a default description.
        type: parameters
      dateTime:
        description: This is a default description.
        type: parameters
      timeZone:
        description: This is a default description.
        type: parameters
  EventReminder:
    properties:
      method:
        description: This is a default description.
        type: parameters
      minutes:
        description: This is a default description.
        type: parameters
  Events:
    properties:
      accessRole:
        description: This is a default description.
        type: parameters
      defaultReminders:
        description: This is a default description.
        type: parameters
      description:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      nextSyncToken:
        description: This is a default description.
        type: parameters
      summary:
        description: This is a default description.
        type: parameters
      timeZone:
        description: This is a default description.
        type: parameters
  FreeBusyCalendar:
    properties:
      busy:
        description: This is a default description.
        type: parameters
      errors:
        description: This is a default description.
        type: parameters
  FreeBusyGroup:
    properties:
      calendars:
        description: This is a default description.
        type: parameters
      errors:
        description: This is a default description.
        type: parameters
  FreeBusyRequest:
    properties:
      calendarExpansionMax:
        description: This is a default description.
        type: parameters
      groupExpansionMax:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      timeMax:
        description: This is a default description.
        type: parameters
      timeMin:
        description: This is a default description.
        type: parameters
      timeZone:
        description: This is a default description.
        type: parameters
  FreeBusyRequestItem:
    properties:
      id:
        description: This is a default description.
        type: parameters
  FreeBusyResponse:
    properties:
      calendars:
        description: This is a default description.
        type: parameters
      groups:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      timeMax:
        description: This is a default description.
        type: parameters
      timeMin:
        description: This is a default description.
        type: parameters
  Setting:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  Settings:
    properties:
      etag:
        description: This is a default description.
        type: parameters
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
      nextSyncToken:
        description: This is a default description.
        type: parameters
  TimePeriod:
    properties:
      end:
        description: This is a default description.
        type: parameters
      start:
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