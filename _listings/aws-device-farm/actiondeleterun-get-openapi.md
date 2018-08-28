---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 0
info:
  title: AWS Device Farm API Delete Run
  version: 1.0.0
  description: Deletes the run, given the run ARN.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteRun:
    get:
      summary: Delete Run
      description: Deletes the run, given the run ARN.
      operationId: deleteRun
      x-api-path-slug: actiondeleterun-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) for the run you wish to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
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