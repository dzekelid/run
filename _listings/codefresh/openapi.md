---
swagger: "2.0"
x-collection-name: Codefresh
x-complete: 1
info:
  title: Codefresh API
  description: codefresh-api-swagger2-0-specification
  termsOfService: http://www.codefresh.io
  contact:
    name: Codefresh api team
    url: http://www.codefresh.io
  version: 1.0.0
host: g.codefresh.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /compositions/{identifier}/run:
    post:
      summary: Post Compositions Entifier Run
      description: Post compositions entifier run.
      operationId: postCompositionsEntifierRun
      x-api-path-slug: compositionsidentifierrun-post
      parameters:
      - in: path
        name: identifier
        description: id or name of a composition
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Compositions
      - Entifier
      - Run
---