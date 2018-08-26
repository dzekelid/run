---
swagger: "2.0"
x-collection-name: APImetrics
x-complete: 1
info:
  title: APImetrics Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calls/{id}/run:
    post:
      summary: Trigger an API Call to run
      description: Trigger an API Call to run
      operationId: triggerAnAPICallToRun
      x-api-path-slug: callsidrun-post
      parameters:
      - in: body
        name: body
        description: '{     location_id: ,     context: {         foo: 1234,         bar:
          %%RESULT_ID%%,         datum: %%DATETIME%%     } }'
        schema:
          $ref: '#/definitions/holder'
      - in: formData
        name: context
        description: Dictionary of variable names and their values
      - in: path
        name: id
        description: ID string of API Call
      - in: formData
        name: location_id
        description: Location ID of test agent that will make the request
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Calls
      - ""
      - Run
---