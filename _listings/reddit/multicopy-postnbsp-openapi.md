---
swagger: "2.0"
x-collection-name: Reddit
x-complete: 0
info:
  title: Reddit Add Multi Copy
  description: Copy a multi.
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
  /multi/copy:
    post&nbsp;:
      summary: Add Multi Copy
      description: Copy a multi.
      operationId: post&nbsp;MultiCopy
      x-api-path-slug: multicopy-postnbsp
      parameters:
      - in: query
        name: display_name
        description: a string no longer than 50 characters
        type: string
      - in: query
        name: from
        description: multireddit url path
        type: string
      - in: query
        name: to
        description: destination multireddit url path
        type: string
      - in: query
        name: uh / X-Modhash header
        description: a modhash
        type: string
      responses:
        200:
          description: OK
      tags:
      - Multi
      - Copy
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