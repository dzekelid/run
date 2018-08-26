{
  "info": {
    "name": "AWS Data Pipeline API Report Task Runner Heartbeat",
    "_postman_id": "aebc51f0-6b6d-44c0-96df-1659622fd536",
    "description": "Task runners call ReportTaskRunnerHeartbeat every 15 minutes to indicate that they are operational.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tasks",
      "item": [
        {
          "id": "1870cfd2-5487-4f6b-8e0c-7d233c0a162d",
          "name": "pollForTask",
          "request": {
            "url": "http://example.com/api/?Action=PollForTask?hostname=hostname&instanceIdentity=instanceIdentity&workerGroup=workerGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Task runners call PollForTask to receive a task to perform from AWS Data Pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a82f589-7261-4bee-9c21-cfd17fd5e6fb"
            }
          ]
        },
        {
          "id": "9dc9125d-5664-497b-93f6-c63297fb71d7",
          "name": "reportTaskProgress",
          "request": {
            "url": "http://example.com/api/?Action=ReportTaskProgress?fields=fields&taskId=taskId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Task runners call ReportTaskProgress when assigned a task to acknowledge that it has the task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbd13f42-1012-45d8-afca-ff24a597ec40"
            }
          ]
        }
      ]
    },
    {
      "name": "Task Runner Hearbeat",
      "item": [
        {
          "id": "0e569198-3507-4d94-b590-4312f3409e1a",
          "name": "reportTaskRunnerHeartbeat",
          "request": {
            "url": "http://example.com/api/?Action=ReportTaskRunnerHeartbeat?hostname=hostname&taskrunnerId=taskrunnerId&workerGroup=workerGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Task runners call ReportTaskRunnerHeartbeat every 15 minutes to indicate that they are operational."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66afbad9-86c3-43e3-8faa-c7e0f289939c"
            }
          ]
        }
      ]
    }
  ]
}