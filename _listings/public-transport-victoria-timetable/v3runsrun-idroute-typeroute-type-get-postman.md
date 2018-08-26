{
  "info": {
    "name": "PTV Timetable API - Version 3 Get V3 Runs Run Route Type Route Type",
    "_postman_id": "0159ff30-f07e-42b3-b431-17dbe0049bd3",
    "description": "View the trip/service run for a specific run id and route type.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Departures",
      "item": [
        {
          "id": "41cf7829-c8c8-4bda-a604-2764ceb1dc8b",
          "name": "Departures_GetForStop",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/departures/route_type/:route_type/stop/:stop_id"
              ],
              "query": [
                {
                  "key": "date_utc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "direction_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "gtfs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_cancelled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "max_results",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "platform_numbers",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "stop_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View departures for all routes from a stop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e770e9b5-ac22-4516-a2d3-61109e619810"
            }
          ]
        },
        {
          "id": "e082326d-f8cf-47b9-a8d5-4cfae5af9769",
          "name": "Departures_GetForStopAndRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/departures/route_type/:route_type/stop/:stop_id/route/:route_id"
              ],
              "query": [
                {
                  "key": "date_utc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "direction_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "gtfs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_cancelled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "max_results",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "stop_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View departures for a specific route from a stop."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec35ad91-e1e6-4c8c-b62a-ed9f6b8261f6"
            }
          ]
        }
      ]
    },
    {
      "name": "Directions",
      "item": [
        {
          "id": "aad01a11-65a8-499b-9fd0-9eeb4a61160b",
          "name": "Directions_ForRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/directions/route/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View directions that a route travels in."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cd0da1f-791d-4daf-a253-a7ca71938a6d"
            }
          ]
        },
        {
          "id": "aec15715-98c8-4c07-aec1-99cd188a0a5e",
          "name": "Directions_ForDirection",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/directions/:direction_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "direction_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all routes for a direction of travel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70a336ad-eb5b-44a3-b721-eafc92ca0d54"
            }
          ]
        },
        {
          "id": "bf489174-95da-4520-ac66-dd42b3b580aa",
          "name": "Directions_ForDirectionAndType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/directions/:direction_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "direction_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all routes of a particular type for a direction of travel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d5e0660-7aab-4cd2-877d-46129184fd5d"
            }
          ]
        }
      ]
    },
    {
      "name": "Disruptions",
      "item": [
        {
          "id": "c30e6b23-fa92-41b5-aec5-4f6b4050940a",
          "name": "Disruptions_GetAllDisruptions",
          "request": {
            "url": "http://timetableapi.ptv.vic.gov.au/v3/disruptions?devid=%7B%7D&disruption_status=%7B%7D&route_types=%7B%7D&signature=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all disruptions for all route types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67c3e701-8932-49a9-9d04-70e89cd23fde"
            }
          ]
        },
        {
          "id": "ca187fba-cc6d-4cef-ac88-a872e4da5ab7",
          "name": "Disruptions_GetDisruptionsByRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/disruptions/route/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "disruption_status",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all disruptions for a particular route."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6806de9b-3369-4bed-9cda-1f6ba35b328d"
            }
          ]
        },
        {
          "id": "fb77c7b8-2681-4836-b025-5227e77e86fe",
          "name": "Disruptions_GetDisruptionById",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/disruptions/:disruption_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "disruption_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View a specific disruption."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c521693-462d-4e49-82d7-d262365b555f"
            }
          ]
        }
      ]
    },
    {
      "name": "Pattern",
      "item": [
        {
          "id": "e18e2253-60fa-49af-9876-9241e863d543",
          "name": "Patterns_GetPatternByRun",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/pattern/run/:run_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "date_utc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "stop_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "run_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View the stopping pattern for a specific trip/service run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "451c6762-0a5b-4f87-b550-8fc06eb488a7"
            }
          ]
        }
      ]
    },
    {
      "name": "Route",
      "item": [
        {
          "id": "4c8be04d-fd29-48db-9bf8-62f50f16610d",
          "name": "RouteTypes_GetRouteTypes",
          "request": {
            "url": "http://timetableapi.ptv.vic.gov.au/v3/route_types?devid=%7B%7D&signature=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all route types and their names."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52380a67-29aa-41b3-98d5-748ae182eff2"
            }
          ]
        }
      ]
    },
    {
      "name": "Routes",
      "item": [
        {
          "id": "d60ed314-705b-4de7-9a6f-84a5f61953ff",
          "name": "Routes_OneOrMoreRoutes",
          "request": {
            "url": "http://timetableapi.ptv.vic.gov.au/v3/routes?devid=%7B%7D&route_name=%7B%7D&route_types=%7B%7D&signature=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View route names and numbers for all routes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f161b34b-db3e-4428-ae69-d84844becdb6"
            }
          ]
        },
        {
          "id": "d679cfc9-9085-4724-b651-f35d4a8b3301",
          "name": "Routes_RouteFromId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/routes/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View route name and number for specific route id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86066dc3-07a0-48ca-8224-befcbedfb57f"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "f70d80f2-f2ce-4768-a2f7-4ff75a617d7b",
          "name": "Runs_ForRoute",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/route/:route_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all trip/service runs for a specific route id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34b356a2-2e4f-478f-a4a8-3e6ed4258cd4"
            }
          ]
        },
        {
          "id": "224f2d1a-31ba-445b-a813-379e59905b31",
          "name": "Runs_ForRouteAndRouteType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/route/:route_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all trip/service runs for a specific route id and route type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4356b85-3b5e-4c1c-8e84-de59313f4071"
            }
          ]
        },
        {
          "id": "0441d03b-5c3b-4010-823c-c39d134d0f26",
          "name": "Runs_ForRun",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/:run_id"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "run_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View all trip/service runs for a specific run id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4246f054-3594-4bb5-aafa-fefa9b2b44ab"
            }
          ]
        },
        {
          "id": "4ed438cd-6936-4dde-b681-dbe1df81ccfa",
          "name": "Runs_ForRunAndRouteType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "timetableapi.ptv.vic.gov.au",
              "path": [
                "v3/runs/:run_id/route_type/:route_type"
              ],
              "query": [
                {
                  "key": "devid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "signature",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "route_type",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "run_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "View the trip/service run for a specific run id and route type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bb79a69-1d68-4381-b8df-758fb24dadcd"
            }
          ]
        }
      ]
    }
  ]
}