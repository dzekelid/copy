swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 1
info:
  title: AWS ElastiCache API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CopySnapshot:
    get:
      summary: Copy Snapshot
      description: Makes a copy of an existing snapshot.
      operationId: copySnapshot
      x-api-path-slug: actioncopysnapshot-get
      parameters:
      - in: query
        name: SourceSnapshotName
        description: The name of an existing snapshot from which to make a copy
        type: string
      - in: query
        name: TargetBucket
        description: The Amazon S3 bucket to which the snapshot is exported
        type: string
      - in: query
        name: TargetSnapshotName
        description: A name for the snapshot copy
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots