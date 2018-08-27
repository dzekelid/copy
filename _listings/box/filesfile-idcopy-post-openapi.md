---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Copy File
  description: Used to create a copy of a file in another folder. The original version
    of the file will not be altered.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{FILE_ID}/copy:
    post:
      summary: Copy File
      description: Used to create a copy of a file in another folder. The original
        version of the file will not be altered.
      operationId: copyFile
      x-api-path-slug: filesfile-idcopy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FILE_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
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