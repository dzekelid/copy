---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Create Snapshot Copy Grant
  version: 1.0.0
  description: |-
    Creates a snapshot copy grant that permits Amazon Redshift to use a customer master key
                (CMK) from AWS Key Management Service (AWS KMS) to encrypt copied snapshots in a
                destination region.
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
  /?Action=CreateSnapshotCopyGrant:
    get:
      summary: Create Snapshot Copy Grant
      description: |-
        Creates a snapshot copy grant that permits Amazon Redshift to use a customer master key
                    (CMK) from AWS Key Management Service (AWS KMS) to encrypt copied snapshots in a
                    destination region.
      operationId: createSnapshotCopyGrant
      x-api-path-slug: actioncreatesnapshotcopygrant-get
      parameters:
      - in: query
        name: KmsKeyId
        description: The unique identifier of the customer master key (CMK) to which
          to grant Amazon Redshift            permission
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant
        type: string
      - in: query
        name: Tags.Tag.N
        description: A list of tag instances
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