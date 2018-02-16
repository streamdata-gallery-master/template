---
swagger: "2.0"
info:
  title: Knoema
  description: You don&rsquo;t need to be a developer to get started. We made a number
    of useful platform features available as ready to use widgets. You can put a dashboard
    or presentation with any visualization/content you like and then embed it in your
    site or blog in a few minutes.  Such an approach requires no programming skills
    at all, just basic understanding of HTML. Refer to Widgets sections for more information
    on this topic. Knoema is a truly open platform.  In addition to our own APIs we
    support several formats widely acknowledged by industry such as OData and SDMX.  If
    you already have tools/clients utilizing data in these formats you can add Knoema
    support very easily. More information can be found in Open Data section. For enthusiasts
    and hardcore developers Knoema offers extensive Knoema API providing access to
    all platform capabilities. Start with getting familiar with core Knoema concepts.
    Then proceed to Applications section to find step-by-step tutorials, detailed
    documentation and sample apps.
  version: 1.0.0
host: knoema.com
basePath: /api/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /frontend/tags:
    get:
      summary: List of tags
      description: Lists out all the public tags present in the system
      operationId: getTags
      responses:
        200:
          description: OK
      tags:
      - Tags
definitions: []
---