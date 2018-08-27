swagger: "2.0"
x-collection-name: Reddit
x-complete: 1
info:
  title: Reddit
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