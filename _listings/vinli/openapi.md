swagger: "2.0"
x-collection-name: Vinli
x-complete: 1
info:
  title: Vinli
  description: todo-add-description
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dummies/01e668ba-6967-4536-9f72-cc28ff18d7b6/runs:
    post:
      summary: Create a Dummy Run
      description: Create a dummy run.
      operationId: Dummies01e668ba696745369f72Cc28ff18d7b6RunsPost
      x-api-path-slug: dummies01e668ba696745369f72cc28ff18d7b6runs-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Dummy
      - Run
  /dummies/01e668ba-6967-4536-9f72-cc28ff18d7b6/runs/_current:
    get:
      summary: Get Current Run
      description: Get current run.
      operationId: Dummies01e668ba696745369f72Cc28ff18d7b6RunsCurrentGet
      x-api-path-slug: dummies01e668ba696745369f72cc28ff18d7b6runs-current-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Current
      - Run
    delete:
      summary: Delete a Run
      description: Delete a run.
      operationId: Dummies01e668ba696745369f72Cc28ff18d7b6RunsCurrentDelete
      x-api-path-slug: dummies01e668ba696745369f72cc28ff18d7b6runs-current-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Run