---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 0
info:
  title: AWS Inspector API Start Assessment Run
  version: 1.0.0
  description: Starts the assessment run specified by the ARN of the assessment template.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteAssessmentRun:
    get:
      summary: Delete Assessment Run
      description: |-
        Deletes the assessment run that is specified by the ARN of the assessment
                 run.
      operationId: deleteAssessmentRun
      x-api-path-slug: actiondeleteassessmentrun-get
      parameters:
      - in: query
        name: assessmentRunArn
        description: The ARN that specifies the assessment run that you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assessment Runs
  /?Action=DescribeAssessmentRuns:
    get:
      summary: Describe Assessment Runs
      description: |-
        Describes the assessment runs that are specified by the ARNs of the assessment
                 runs.
      operationId: describeAssessmentRuns
      x-api-path-slug: actiondescribeassessmentruns-get
      parameters:
      - in: query
        name: assessmentRunArns
        description: The ARN that specifies the assessment run that you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assessment Runs
  /?Action=ListAssessmentRunAgents:
    get:
      summary: List Assessment Run Agents
      description: |-
        Lists the agents of the assessment runs that are specified by the ARNs of the
                 assessment runs.
      operationId: listAssessmentRunAgents
      x-api-path-slug: actionlistassessmentrunagents-get
      parameters:
      - in: query
        name: assessmentRunArn
        description: The ARN that specifies the assessment run whose agents you want
          to list
        type: string
      - in: query
        name: filter
        description: You can use this parameter to specify a subset of data to be
          included in the actions         response
        type: string
      - in: query
        name: maxResults
        description: You can use this parameter to indicate the maximum number of
          items that you want in         the response
        type: string
      - in: query
        name: nextToken
        description: You can use this parameter when paginating results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assessment Run Agents
  /?Action=ListAssessmentRuns:
    get:
      summary: List Assessment Runs
      description: |-
        Lists the assessment runs that correspond to the assessment templates that are
                 specified by the ARNs of the assessment templates.
      operationId: listAssessmentRuns
      x-api-path-slug: actionlistassessmentruns-get
      parameters:
      - in: query
        name: assessmentTemplateArns
        description: The ARNs that specify the assessment templates whose assessment
          runs you want to         list
        type: string
      - in: query
        name: filter
        description: You can use this parameter to specify a subset of data to be
          included in the actions         response
        type: string
      - in: query
        name: maxResults
        description: You can use this parameter to indicate the maximum number of
          items that you want in         the response
        type: string
      - in: query
        name: nextToken
        description: You can use this parameter when paginating results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assessment Runs
  /?Action=StartAssessmentRun:
    get:
      summary: Start Assessment Run
      description: Starts the assessment run specified by the ARN of the assessment
        template.
      operationId: startAssessmentRun
      x-api-path-slug: actionstartassessmentrun-get
      parameters:
      - in: query
        name: assessmentRunName
        description: You can specify the name for the assessment run
        type: string
      - in: query
        name: assessmentTemplateArn
        description: The ARN of the assessment template of the assessment run that
          you want to         start
        type: string
      responses:
        200:
          description: OK
      tags:
      - Assessment Runs
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