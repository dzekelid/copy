---
swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 0
info:
  title: Amazon Redshift API Disable Snapshot Copy
  version: 1.0.0
  description: |-
    Disables the automatic copying of snapshots from one region to another region for a
                specified cluster.
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
  /?Action=DeleteSnapshotCopyGrant:
    get:
      summary: Delete Snapshot Copy Grant
      description: Deletes the specified snapshot copy grant.
      operationId: deleteSnapshotCopyGrant
      x-api-path-slug: actiondeletesnapshotcopygrant-get
      parameters:
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DescribeSnapshotCopyGrants:
    get:
      summary: Describe Snapshot Copy Grants
      description: |-
        Returns a list of snapshot copy grants owned by the AWS account in the destination
                    region.
      operationId: describeSnapshotCopyGrants
      x-api-path-slug: actiondescribesnapshotcopygrants-get
      parameters:
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: SnapshotCopyGrantName
        description: The name of the snapshot copy grant
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching resources
          that are            associated with the specified key or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          resources that are            associated with the specified value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
  /?Action=DisableSnapshotCopy:
    get:
      summary: Disable Snapshot Copy
      description: |-
        Disables the automatic copying of snapshots from one region to another region for a
                    specified cluster.
      operationId: disableSnapshotCopy
      x-api-path-slug: actiondisablesnapshotcopy-get
      parameters:
      - in: query
        name: ClusterIdentifier
        description: The unique identifier of the source cluster that you want to
          disable copying of            snapshots to a destination region
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