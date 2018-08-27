---
swagger: "2.0"
x-collection-name: Dropbox
x-complete: 0
info:
  title: Dropbox Core Copies a file or folder to a new location.
  description: Copies a file or folder to a new location.
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /copy_ref/{root}/{path}:
    get:
      summary: Creates and returns a copy_ref to a file.
      description: |-
        Creates and returns a `copy_ref` to a file.

        This reference string can be used to copy that file to another user's Dropbox by passing it in as the
        `from_copy_ref` parameter on [/fileops/copy](https://www.dropbox.com/developers/core/docs#fileops-copy).
      operationId: creates-and-returns-a-copy-ref-to-a-filethis-reference-string-can-be-used-to-copy-that-file-to-anoth
      x-api-path-slug: copy-refrootpath-get
      parameters:
      - in: path
        name: path
        description: The path to the file you want a `copy_ref` to refer to
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Copy
      - Root
      - Path
  /fileops/copy:
    post:
      summary: Copies a file or folder to a new location.
      description: Copies a file or folder to a new location.
      operationId: copies-a-file-or-folder-to-a-new-location
      x-api-path-slug: fileopscopy-post
      parameters:
      - in: formData
        name: from_copy_ref
        description: Specifies a `copy_ref` generated from a previous [/copy_ref](https://www
      - in: formData
        name: from_path
        description: Specifies the file or folder to be copied from relative to `root`
      - in: formData
        name: locale
        description: The metadata returned will have its `size` field translated based
          on the given locale
      - in: formData
        name: root
        description: The root relative to which `from_path` and `to_path` are specified
      - in: formData
        name: to_path
        description: Specifies the destination path, *including the new name for the
          file or folder*, relative to `root`
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Fileops
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