swagger: "2.0"
x-collection-name: AWS Server Migration Service
x-complete: 1
info:
  title: AWS Server Migration Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteReplicationJob:
    get:
      summary: Delete Replication Job
      description: The delete-replication-job API is used to delete a ReplicationJob,
        resulting in no further ReplicationRuns.
      operationId: deleteReplicationJob
      x-api-path-slug: actiondeletereplicationjob-get
      parameters:
      - in: query
        name: replicationJobId
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Jobs
  /?Action=GetReplicationRuns:
    get:
      summary: Get Replication Runs
      description: The get-replication-runs API will return all ReplicationRuns for
        a given ReplicationJob.
      operationId: getReplicationRuns
      x-api-path-slug: actiongetreplicationruns-get
      parameters:
      - in: query
        name: maxResults
        description: 'Type: Integer'
        type: string
      - in: query
        name: nextToken
        description: 'Type: String'
        type: string
      - in: query
        name: replicationJobId
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Runs
  /?Action=StartOnDemandReplicationRun:
    get:
      summary: Start On Demand Replication Run
      description: The start-on-demand-replication-run API is used to start a ReplicationRun
        on demand (in addition to those that are scheduled based on your frequency).
      operationId: startOnDemandReplicationRun
      x-api-path-slug: actionstartondemandreplicationrun-get
      parameters:
      - in: query
        name: description
        description: 'Type: String'
        type: string
      - in: query
        name: replicationJobId
        description: 'Type: String'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Replication Runs