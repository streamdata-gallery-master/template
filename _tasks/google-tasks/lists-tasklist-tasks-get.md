---
swagger: "2.0"
info:
  title: Tasks
  description: Lets you manage your tasks and task lists.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tasks/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/{tasklist}/tasks:
    get:
      summary: ""
      description: Returns all tasks in the specified task list
      operationId: tasks.tasks.list
      parameters:
      - in: query
        name: completedMax
        description: Upper bound for a task's completion date (as a RFC 3339 timestamp)
          to filter by
      - in: query
        name: completedMin
        description: Lower bound for a task's completion date (as a RFC 3339 timestamp)
          to filter by
      - in: query
        name: dueMax
        description: Upper bound for a task's due date (as a RFC 3339 timestamp) to
          filter by
      - in: query
        name: dueMin
        description: Lower bound for a task's due date (as a RFC 3339 timestamp) to
          filter by
      - in: query
        name: maxResults
        description: Maximum number of task lists returned on one page
      - in: query
        name: pageToken
        description: Token specifying the result page to return
      - in: query
        name: showCompleted
        description: Flag indicating whether completed tasks are returned in the result
      - in: query
        name: showDeleted
        description: Flag indicating whether deleted tasks are returned in the result
      - in: query
        name: showHidden
        description: Flag indicating whether hidden tasks are returned in the result
      - in: path
        name: tasklist
        description: Task list identifier
      - in: query
        name: updatedMin
        description: Lower bound for a task's last modification time (as a RFC 3339
          timestamp) to filter by
      responses:
        200:
          description: OK
      tags:
      - ""
definitions:
  Task:
    properties:
      completed:
        description: This is a default description.
        type: put
      deleted:
        description: This is a default description.
        type: put
      due:
        description: This is a default description.
        type: put
      etag:
        description: This is a default description.
        type: put
      hidden:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      links:
        description: This is a default description.
        type: put
      notes:
        description: This is a default description.
        type: put
      parent:
        description: This is a default description.
        type: put
  TaskList:
    properties:
      etag:
        description: This is a default description.
        type: put
      id:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      selfLink:
        description: This is a default description.
        type: put
      title:
        description: This is a default description.
        type: put
      updated:
        description: This is a default description.
        type: put
  TaskLists:
    properties:
      etag:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
        description: This is a default description.
        type: put
  Tasks:
    properties:
      etag:
        description: This is a default description.
        type: put
      items:
        description: This is a default description.
        type: put
      kind:
        description: This is a default description.
        type: put
      nextPageToken:
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