swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
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
  /folders/{FOLDER_ID}/copy:
    post:
      summary: Copy Folder
      description: Used to create a copy of a folder in another folder. The original
        version of the folder will not be altered.
      operationId: copyFolder
      x-api-path-slug: foldersfolder-idcopy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      - in: path
        name: FOLDER_ID
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Folders
      - Folder
      - ""
      - Copy