---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Copy Cluster Snapshot
  version: 1.0.0
  description: Copies the specified automated cluster snapshot to a new manual cluster
    snapshot.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CopyClusterSnapshot:
    get:
      summary: Copy Cluster Snapshot
      description: Copies the specified automated cluster snapshot to a new manual
        cluster snapshot.
      operationId: copyClusterSnapshot
      x-api-path-slug: actioncopyclustersnapshot-get
      parameters:
      - in: query
        name: SourceSnapshotClusterIdentifier
        description: The identifier of the cluster the source snapshot was created
          from
        type: string
      - in: query
        name: SourceSnapshotIdentifier
        description: The identifier for the source snapshot
        type: string
      - in: query
        name: TargetSnapshotIdentifier
        description: The identifier given to the new manual snapshot
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
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