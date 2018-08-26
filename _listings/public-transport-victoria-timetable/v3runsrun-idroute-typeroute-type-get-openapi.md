---
swagger: "2.0"
x-collection-name: Public Transport Victoria Timetable
x-complete: 0
info:
  title: PTV Timetable API - Version 3 Get V3 Runs Run Route Type Route Type
  description: View the trip/service run for a specific run id and route type.
  termsOfService: http://ptv.vic.gov.au/ptv-timetable-api/
  contact:
    name: Public Transport Victoria
    url: http://ptv.vic.gov.au/digital
  version: v3
host: timetableapi.ptv.vic.gov.au
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/pattern/run/{run_id}/route_type/{route_type}:
    get:
      summary: Get V3 Pattern Run Run Route Type Route Type
      description: View the stopping pattern for a specific trip/service run.
      operationId: Patterns_GetPatternByRun
      x-api-path-slug: v3patternrunrun-idroute-typeroute-type-get
      parameters:
      - in: query
        name: date_utc
        description: Filter by the date and time of the request (ISO 8601 UTC format)
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: path
        name: run_id
        description: Identifier of a trip/service run; values returned by Runs API
          - /v3/route/{route_id} and Departures API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: stop_id
        description: Filter by stop_id; values returned by Stops API
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Pattern
      - Run
      - Run
      - Id
      - Route
      - Type
      - Route
      - Type
  /v3/runs/{run_id}:
    get:
      summary: Get V3 Runs Run
      description: View all trip/service runs for a specific run id.
      operationId: Runs_ForRun
      x-api-path-slug: v3runsrun-id-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: run_id
        description: Identifier of a trip/service run; values returned by Runs API
          - /v3/route/{route_id} and Departures API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Run
      - Id
  /v3/runs/{run_id}/route_type/{route_type}:
    get:
      summary: Get V3 Runs Run Route Type Route Type
      description: View the trip/service run for a specific run id and route type.
      operationId: Runs_ForRunAndRouteType
      x-api-path-slug: v3runsrun-idroute-typeroute-type-get
      parameters:
      - in: query
        name: devid
        description: Your developer id
      - in: path
        name: route_type
        description: Number identifying transport mode; values returned via RouteTypes
          API
      - in: path
        name: run_id
        description: Identifier of a trip/service run; values returned by Runs API
          - /v3/route/{route_id} and Departures API
      - in: query
        name: signature
        description: Authentication signature for request
      - in: query
        name: token
        description: Please ignore
      responses:
        200:
          description: OK
      tags:
      - Runs
      - Run
      - Id
      - Route
      - Type
      - Route
      - Type
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