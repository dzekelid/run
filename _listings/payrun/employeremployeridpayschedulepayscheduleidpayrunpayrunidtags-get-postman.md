{
  "info": {
    "name": "Pay Run.IO Get all pay run tags",
    "_postman_id": "288ecd88-1182-460d-9708-b9549d710c02",
    "description": "Gets all the tags from the pay run",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Employee",
      "item": [
        {
          "id": "46a88091-f644-4f04-b626-c3d828da2744",
          "name": "GetTagsFromEmployee",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employee/:EmployeeId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the employee"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ab55955-d6ec-4767-ba32-810cd5c8c173"
            }
          ]
        },
        {
          "id": "35fa94e6-a78d-4f11-ae03-c0911a44ec54",
          "name": "GetTagsFromEmployeeRevision",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employee/:EmployeeId/Tags/:EffectiveDate"
              ],
              "variable": [
                {
                  "id": "EffectiveDate",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the employee revision"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d501e30-b52b-49e5-8085-f6470e8609fe"
            }
          ]
        },
        {
          "id": "87afd4ee-d8db-46bb-a943-cb47d237eb73",
          "name": "GetAllEmployeeTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/Employees/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the employee tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b0cda5f-bd29-4e63-8026-6c3b1c753aab"
            }
          ]
        }
      ]
    },
    {
      "name": "Pay",
      "item": [
        {
          "id": "42413104-d0fb-4e0c-a72a-e26863bfea48",
          "name": "GetTagsFromPayCode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PayCode/:PayCodeId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayCodeId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the pay code"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72eb238b-190c-4447-86c8-7fe65e952c5f"
            }
          ]
        },
        {
          "id": "f1ae7165-6c85-4032-9946-3c3edd8b23bb",
          "name": "GetAllPayCodeTags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PayCodes/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the pay code tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f59a6a9e-93c8-4fa3-8508-b8d0fdde5040"
            }
          ]
        },
        {
          "id": "458d2211-2a33-48f2-953c-55d283503de9",
          "name": "GetTagsFromPayRun",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.test.payrun.io",
              "path": [
                "Employer/:EmployerId/PaySchedule/:PayScheduleId/PayRun/:PayRunId/Tags"
              ],
              "variable": [
                {
                  "id": "EmployerId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayRunId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "PayScheduleId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets all the tags from the pay run"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "555ee58a-38a5-41ad-933e-53a093232a9e"
            }
          ]
        }
      ]
    }
  ]
}