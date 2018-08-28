---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Gets the pay run job template
  description: Return the pay run job data object template
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}:
    delete:
      summary: Deletes a pay run
      description: Delete the specified pay run
      operationId: DeletePayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
    get:
      summary: Gets the pay run from the pay schedule
      description: Returns the pay run from the pay schedule
      operationId: GetPayRunFromPaySchedule
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - From
      - Pay
      - Schedule
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/Employee/{EmployeeId}:
    delete:
      summary: Deletes a pay run employee
      description: Delete pay run results for a single employee
      operationId: DeletePayRunEmployee
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidemployeeemployeeid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployeeId
        description: The employees unique identifier
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Employee
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/Employees:
    get:
      summary: Get employees from the pay run
      description: Gets links to all employees included in the specified pay run.
      operationId: GetEmployeesFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidemployees-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Employees
      - From
      - Pay
      - Run
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/ReportLines:
    get:
      summary: Gets the report lines from the specified pay run
      description: Returns all report lines associated with the specified pay run
      operationId: GetReportLinesFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidreportlines-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Report
      - Lines
      - From
      - Specified
      - Pay
      - Run
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/Tag/{TagId}:
    delete:
      summary: Delete pay run tag
      description: Deletes a tag from the pay run
      operationId: DeletePayRunTag
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidtagtagid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Tag
    get:
      summary: Get pay run tag
      description: Gets the tag from the pay run
      operationId: GetTagFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidtagtagid-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Tag
    put:
      summary: Insert pay run tag
      description: Inserts a new tag on the pay run
      operationId: PutPayRunTag
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidtagtagid-put
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      - in: path
        name: TagId
        description: The tag unique identifier
      responses:
        200:
          description: OK
      tags:
      - Insert
      - Pay
      - Run
      - Tag
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRun/{PayRunId}/Tags:
    get:
      summary: Get all pay run tags
      description: Gets all the tags from the pay run
      operationId: GetTagsFromPayRun
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunpayrunidtags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayRunId
        description: The pay runs unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Tags
  /Employer/{EmployerId}/PaySchedule/{PayScheduleId}/PayRuns/Tags:
    get:
      summary: Get all pay run tags
      description: Gets all the pay run tags
      operationId: GetAllPayRunTags
      x-api-path-slug: employeremployeridpayschedulepayscheduleidpayrunstags-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: EmployerId
        description: The employers unique identifier
      - in: path
        name: PayScheduleId
        description: The pay schedules unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Tags
  /Jobs/PayRuns/{JobId}:
    delete:
      summary: Delete the pay run job
      description: Deletes the the payrun job
      operationId: DeletePayRunJob
      x-api-path-slug: jobspayrunsjobid-delete
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
  /Jobs/PayRuns/{JobId}/Info:
    get:
      summary: Get the pay run job information
      description: Return the the payrun job information
      operationId: GetPayRunJobInfo
      x-api-path-slug: jobspayrunsjobidinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Information
  /Jobs/PayRuns/{JobId}/Progress:
    get:
      summary: Get the pay run job progress
      description: Return the the payrun job progress
      operationId: GetPayRunJobProgress
      x-api-path-slug: jobspayrunsjobidprogress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Progress
  /Jobs/PayRuns/{JobId}/Status:
    get:
      summary: Get the pay run job status
      description: Return the the payrun job status
      operationId: GetPayRunJobStatus
      x-api-path-slug: jobspayrunsjobidstatus-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      - in: path
        name: JobId
        description: The job unique identifier
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Status
  /Templates/payrun:
    get:
      summary: Gets the pay run template
      description: Return the pay run data object template
      operationId: GetPayRunTemplate
      x-api-path-slug: templatespayrun-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Template
  /Templates/payrunjob:
    get:
      summary: Gets the pay run job template
      description: Return the pay run job data object template
      operationId: GetPayRunJobTemplate
      x-api-path-slug: templatespayrunjob-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Pay
      - Run
      - Job
      - Template
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