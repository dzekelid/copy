---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Message Copy
  description: 'message: copy Copy a message to a folder.'
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/mailFolders/{id}/copy:
    post:
      summary: Mail Folder Copy
      description: 'mailFolder: copy Copy a mailfolder and its contents to another
        mailfolder.'
      operationId: MailFolder:Copy
      x-api-path-slug: memailfoldersidcopy-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
      - Copy
  /users/{id | userPrincipalName}/mailFolders/{id}/copy:
    post:
      summary: Mail Folder Copy
      description: 'mailFolder: copy Copy a mailfolder and its contents to another
        mailfolder.'
      operationId: MailFolder:Copy
      x-api-path-slug: usersid--userprincipalnamemailfoldersidcopy-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Mail
      - Folder
      - Copy
  /me/messages/{id}/copy:
    post:
      summary: Message Copy
      description: 'message: copy Copy a message to a folder.'
      operationId: Message:Copy
      x-api-path-slug: memessagesidcopy-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message
      - Copy
  /users/{id | userPrincipalName}/messages/{id}/copy:
    post:
      summary: Message Copy
      description: 'message: copy Copy a message to a folder.'
      operationId: Message:Copy
      x-api-path-slug: usersid--userprincipalnamemessagesidcopy-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Message
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