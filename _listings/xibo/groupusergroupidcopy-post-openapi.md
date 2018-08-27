---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Copy User Group
  description: Copy an user group, optionally copying the group members
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dataset/copy/{dataSetId}:
    post:
      summary: Copy DataSet
      description: Copy a DataSet
      operationId: dataSetCopy
      x-api-path-slug: datasetcopydatasetid-post
      parameters:
      - in: formData
        name: code
        description: A code for this DataSet
      - in: formData
        name: dataSet
        description: The DataSet Name
      - in: path
        name: dataSetId
        description: The DataSet ID
      - in: formData
        name: description
        description: A description of this DataSet
      responses:
        200:
          description: OK
      tags:
      - Copy
      - DataSet
  /layout/copy/{layoutId}:
    post:
      summary: Copy Layout
      description: Copy a Layout, providing a new name if applicable
      operationId: layoutCopy
      x-api-path-slug: layoutcopylayoutid-post
      parameters:
      - in: formData
        name: copyMediaFiles
        description: Flag indicating whether to make new Copies of all Media Files
          assigned to the Layout being Copied
      - in: formData
        name: description
        description: The Description for the new Layout
      - in: path
        name: layoutId
        description: The Layout ID to Copy
      - in: formData
        name: name
        description: The name for the new Layout
      responses:
        200:
          description: OK
      tags:
      - Copy
      - Layout
  /group/{userGroupId}/copy:
    post:
      summary: Copy User Group
      description: Copy an user group, optionally copying the group members
      operationId: userGroupCopy
      x-api-path-slug: groupusergroupidcopy-post
      parameters:
      - in: formData
        name: copyMembers
        description: Flag indicating whether to copy group members
      - in: formData
        name: group
        description: The Group Name
      - in: path
        name: userGroupId
        description: The User Group ID to Copy
      responses:
        200:
          description: OK
      tags:
      - Copy
      - User
      - Group
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