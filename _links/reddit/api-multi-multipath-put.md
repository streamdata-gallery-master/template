---
swagger: "2.0"
info:
  title: Reddit
  description: The Reddit API allows you to access the user submitted and rated stories
    on reddit.com. It also provides advanced functionality, including user account
    information and sub-reddit moderation.
  version: 1.0.0
host: www.reddit.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/multi/multipath:
    put:
      summary: Put&nbsp; Api Multi Multipath
      description: Create or update a multi
      operationId: multis
      parameters:
      - in: query
        name: expand_srs
        description: boolean value
        type: string
      - in: query
        name: model
        description: 'json data:{  &quot;description_md&quot;: raw markdown text,  &quot;display_name&quot;:
          a string no longer than 50 characters,  &quot;icon_name&quot;: one of (`art
          and design`, `ask`, `books`, `business`, `cars`, `comics`, `cute animals`,
          `diy`, `entertainment`, `food and drink`, `funny`, `games`, `grooming`,
          `health`, `life advice`, `military`, `models pinup`, `music`, `news`, `philosophy`,
          `pictures and gifs`, `science`, `shopping`, `sports`, `style`, `tech`, `travel`,
          `unusual stories`, `video`, ``, `None`),  &quot;key_color&quot;: a 6-digit
          rgb hex color, e'
        type: string
      - in: query
        name: multipath
        description: multireddit url path
        type: string
      - in: query
        name: uh / X-Modhash header
        description: a modhash
        type: string
      responses:
        200:
          description: OK
      tags:
      - links
      - api
      - multi
      - multipath
definitions: []
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