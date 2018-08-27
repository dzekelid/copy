swagger: "2.0"
x-collection-name: AWS S3
x-complete: 1
info:
  title: No Title
  version: 1.0.0
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