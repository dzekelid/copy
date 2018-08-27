---
swagger: "2.0"
x-collection-name: Microsoft Office 365
x-complete: 0
info:
  title: Microsoft Office 365 Parameters Messages Message Copy
  description: Parameters messages message  copy
  version: 1.0.0
host: outlook.office365.com
basePath: /ews/odata/Me
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Messages{message_id}/Copy:
    post:
      summary: Add Messages Message Copy
      description: Post messages message  copy
      operationId: postMessagesMessageCopy
      x-api-path-slug: messagesmessage-idcopy-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
      - ""
      - Copy
    parameters:
      summary: Parameters Messages Message Copy
      description: Parameters messages message  copy
      operationId: parametersMessagesMessageCopy
      x-api-path-slug: messagesmessage-idcopy-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Message
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