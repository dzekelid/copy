---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 PUT Object - Copy
  version: 1.0.0
  description: This implementation of the PUT operation creates a copy of an object
    that is      already stored in Amazon S3
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /destinationObject:
    put:
      summary: PUT Object - Copy
      description: This implementation of the PUT operation creates a copy of an object
        that is      already stored in Amazon S3
      operationId: put-object--copy
      x-api-path-slug: destinationobject-put
      responses:
        200:
          description: OK
      tags:
      - Object
      - '-'
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