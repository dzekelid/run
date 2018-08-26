---
swagger: "2.0"
x-collection-name: AWS Device Farm
x-complete: 1
info:
  title: AWS Device Farm API
  version: 1.0.0
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
  /?Action=GetRun:
    get:
      summary: Get Run
      description: Gets information about a run.
      operationId: getRun
      x-api-path-slug: actiongetrun-get
      parameters:
      - in: query
        name: arn
        description: The runs ARN
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
  /?Action=ListRuns:
    get:
      summary: List Runs
      description: Gets information about runs, given an AWS Device Farm project ARN.
      operationId: listRuns
      x-api-path-slug: actionlistruns-get
      parameters:
      - in: query
        name: arn
        description: The Amazon Resource Name (ARN) of the project for which you want
          to list runs
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous call to this
          operation, which can be used to return the next set of items in the list
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
  /?Action=ScheduleRun:
    get:
      summary: Schedule Run
      description: Schedules a run.
      operationId: scheduleRun
      x-api-path-slug: actionschedulerun-get
      parameters:
      - in: query
        name: appArn
        description: The ARN of the app to schedule a run
        type: string
      - in: query
        name: configuration
        description: Information about the settings for the run to be scheduled
        type: string
      - in: query
        name: devicePoolArn
        description: The ARN of the device pool for the run to be scheduled
        type: string
      - in: query
        name: name
        description: The name for the run to be scheduled
        type: string
      - in: query
        name: projectArn
        description: The ARN of the project for the run to be scheduled
        type: string
      - in: query
        name: test
        description: Information about the test for the run to be scheduled
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
  /?Action=StopRun:
    get:
      summary: Stop Run
      description: Initiates a stop request for the current test run.
      operationId: stopRun
      x-api-path-slug: actionstoprun-get
      parameters:
      - in: query
        name: arn
        description: Represents the Amazon Resource Name (ARN) of the Device Farm
          run you wish to stop
        type: string
      responses:
        200:
          description: OK
      tags:
      - Runs
---