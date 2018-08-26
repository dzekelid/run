---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/admin/searchsync/start:
    post:
      summary: Create and run as search sync request
      description: Create and run as search sync request.
      operationId: SearchSync_CreateAndStartWorkflowSyncBymigrationId
      x-api-path-slug: apiadminsearchsyncstart-post
      parameters:
      - in: query
        name: migrationId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Run
      - As
      - Search
      - Sync
      - Request
---