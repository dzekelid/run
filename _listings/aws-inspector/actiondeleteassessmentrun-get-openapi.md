---
swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 0
info:
  title: AWS Inspector API Delete Assessment Run
  version: 1.0.0
  description: |-
    Deletes the assessment run that is specified by the ARN of the assessment
             run.
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