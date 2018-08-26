---
swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 0
info:
  title: Global Change Information System API Get a representation of a model run.
  description: Get JSON which represents the structure of a model run.
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /model_run/{model_identifier}/{scenario_identifier}/{range_start}/{range_end}/{spatial_resolution}/{time_resolution}/{sequence}:
    get:
      summary: Get a representation of a model run.
      description: Get JSON which represents the structure of a model run.
      operationId: get-json-which-represents-the-structure-of-a-model-run
      x-api-path-slug: model-runmodel-identifierscenario-identifierrange-startrange-endspatial-resolutiontime-resolutionsequence-get
      parameters:
      - in: path
        name: model_identifier
        description: model_identifier description
      - in: path
        name: range_end
        description: range_end description
      - in: path
        name: range_start
        description: range_start description
      - in: path
        name: scenario_identifier
        description: scenario_identifier description
      - in: path
        name: sequence
        description: sequence description
      - in: path
        name: spatial_resolution
        description: spatial_resolution description
      - in: path
        name: time_resolution
        description: time_resolution description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - Model
      - Run
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