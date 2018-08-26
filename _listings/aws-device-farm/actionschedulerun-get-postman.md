{
  "info": {
    "name": "AWS Device Farm API Schedule Run",
    "_postman_id": "cdac453b-99b8-4bdf-99e3-6a70119d0379",
    "description": "Schedules a run.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "570d96f6-a75c-428c-ba30-7233cabe5222",
          "name": "createDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=CreateDevicePool?description=description&name=name&projectArn=projectArn&rules=rules",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e8a7145-bec7-45b2-bcae-6e1782b3757d"
            }
          ]
        },
        {
          "id": "2506a650-ec96-472f-9bcb-07ea4c7f7ac2",
          "name": "deleteDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a device pool given the pool ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31f648b0-35c3-493a-8592-7d77f00fc0d4"
            }
          ]
        },
        {
          "id": "9373cc53-c3d9-4207-b10e-f0946a9dd0e5",
          "name": "getDevicePool",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePool?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbd606cd-ad9b-498b-be6a-e814d09d9c04"
            }
          ]
        },
        {
          "id": "9389df18-2f96-467f-bf7a-b013d03d6cce",
          "name": "getDevicePoolCompatibility",
          "request": {
            "url": "http://example.com/api/?Action=GetDevicePoolCompatibility?appArn=appArn&devicePoolArn=devicePoolArn&testType=testType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about compatibility with a device pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84a6a7f8-0018-441e-9b3e-4a68d0b3e0d1"
            }
          ]
        },
        {
          "id": "ffeae60b-97c5-4e8e-b8f7-adfd37cca0d2",
          "name": "listDevicePools",
          "request": {
            "url": "http://example.com/api/?Action=ListDevicePools?arn=arn&nextToken=nextToken&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about device pools."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74b248bb-9b04-48a3-a168-bb4a8937d781"
            }
          ]
        }
      ]
    },
    {
      "name": "Project",
      "item": [
        {
          "id": "8ce6098b-7c82-47ed-ad19-e3091c896e7a",
          "name": "createProject",
          "request": {
            "url": "http://example.com/api/?Action=CreateProject?name=name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efc6dc28-0037-48ed-a826-f7a0bdfdfadf"
            }
          ]
        }
      ]
    },
    {
      "name": "Remote Access Sessions",
      "item": [
        {
          "id": "3a02d428-68a7-4530-a104-f6680081c3c1",
          "name": "createRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=CreateRemoteAccessSession?configuration=configuration&deviceArn=deviceArn&name=name&projectArn=projectArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Specifies and starts a remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33b1ce49-efac-4080-996e-f629e2736ac7"
            }
          ]
        },
        {
          "id": "a14e1f08-3ed6-4070-884f-648a88c7487e",
          "name": "deleteRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a completed remote access session and its results."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84da7d03-b191-4024-b81d-a4959a0afd27"
            }
          ]
        },
        {
          "id": "c35c99de-e1b2-4210-9054-56558d0dad49",
          "name": "getRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=GetRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a link to a currently running remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0820cb9-4f6e-424b-b5ec-c5ceebb7a70a"
            }
          ]
        },
        {
          "id": "038163df-29db-46cf-bb98-d2bc1dbdfd90",
          "name": "installToRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=InstallToRemoteAccessSession?appArn=appArn&remoteAccessSessionArn=remoteAccessSessionArn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Installs an application to the device in a remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c0e5f6c-2a19-4b82-907c-3e305cc1ff03"
            }
          ]
        },
        {
          "id": "b02e2ddf-cf6d-4dac-b02c-fed4d4138320",
          "name": "listRemoteAccessSessions",
          "request": {
            "url": "http://example.com/api/?Action=ListRemoteAccessSessions?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all currently running remote access sessions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9747cd43-db6e-4773-ae87-d5b00295ee8b"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "7045935d-3033-4d5e-849a-b31e336005be",
          "name": "createUpload",
          "request": {
            "url": "http://example.com/api/?Action=CreateUpload?contentType=contentType&name=name&projectArn=projectArn&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Uploads an app or test scripts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba8191cf-5156-4ebf-ac96-0b6a3fdc8ffe"
            }
          ]
        },
        {
          "id": "91c7463f-7d2b-4f7b-8aae-268c0b226780",
          "name": "getUpload",
          "request": {
            "url": "http://example.com/api/?Action=GetUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about an upload."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbff17d1-4fab-417e-b148-2bf69084da86"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "f3b48768-acf8-41c0-9b37-ecc8c017a252",
          "name": "deleteProject",
          "request": {
            "url": "http://example.com/api/?Action=DeleteProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Device Farm project, given the project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a8c5118-6a87-4449-ad0e-b3734cfec004"
            }
          ]
        },
        {
          "id": "148659c1-ae1a-46ee-afb8-48cf73560f9e",
          "name": "getProject",
          "request": {
            "url": "http://example.com/api/?Action=GetProject?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a project."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db32d146-273c-425a-92df-be80059aa589"
            }
          ]
        },
        {
          "id": "e3ad5b5d-3d9c-4917-9606-de5f29f6a2e6",
          "name": "listProjects",
          "request": {
            "url": "http://example.com/api/?Action=ListProjects?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about projects."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3ab06cc-b7ce-47ab-859a-13d8937599d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "fd967186-fae2-4e1d-bae6-b030f8596296",
          "name": "deleteRun",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the run, given the run ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1000225b-53db-42aa-9e65-9dcff009a539"
            }
          ]
        },
        {
          "id": "135dcabc-7ecc-4197-ad76-65096f7ca266",
          "name": "getRun",
          "request": {
            "url": "http://example.com/api/?Action=GetRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c880370-f14c-4070-b052-4c06a554e4f5"
            }
          ]
        },
        {
          "id": "6589b8ea-cdaf-427c-b50a-47bf882e4356",
          "name": "listRuns",
          "request": {
            "url": "http://example.com/api/?Action=ListRuns?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about runs, given an AWS Device Farm project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38c794a2-f8c1-4fab-8c12-7eedef3b7ee9"
            }
          ]
        },
        {
          "id": "916f41de-853d-4abc-b10e-1c7fbeeea552",
          "name": "scheduleRun",
          "request": {
            "url": "http://example.com/api/?Action=ScheduleRun?appArn=appArn&configuration=configuration&devicePoolArn=devicePoolArn&name=name&projectArn=projectArn&test=test",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Schedules a run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6183f90e-bf62-458d-9d7a-ca9b0ea40947"
            }
          ]
        }
      ]
    },
    {
      "name": "Uploads",
      "item": [
        {
          "id": "cfe1cef5-37de-4c08-a63e-0fa31bdaf154",
          "name": "deleteUpload",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUpload?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an upload given the upload ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c01cb12d-18e8-41ba-9c44-e86b1a07b8f5"
            }
          ]
        },
        {
          "id": "d0ff2220-f385-483f-9748-92e35d193c5c",
          "name": "listUploads",
          "request": {
            "url": "http://example.com/api/?Action=ListUploads?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about uploads, given an AWS Device Farm project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c90d6c3f-598b-4aeb-af28-d11daa89b9fc"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Settings",
      "item": [
        {
          "id": "048fb5d9-a6fc-4eb2-a478-0a1c06d95965",
          "name": "getAccountSettings",
          "request": {
            "url": "http://example.com/api/?Action=GetAccountSettings?accountSettings=accountSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of unmetered iOS and/or unmetered Android devices that have been purchased by the account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be042e29-547d-4f01-9dda-e9d60f3535f2"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "9284bad9-49b5-4a7f-95c4-c1612a066392",
          "name": "getDevice",
          "request": {
            "url": "http://example.com/api/?Action=GetDevice?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a unique device type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d948977-aad2-4892-b296-0aba11b0428b"
            }
          ]
        },
        {
          "id": "5a79e09e-797b-43c9-9466-3f1aecf1daa1",
          "name": "listDevices",
          "request": {
            "url": "http://example.com/api/?Action=ListDevices?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about unique device types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c92d47e-7de5-40da-8fb1-18779334fd24"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "cbd79b84-9cb1-4d9a-98be-fe983b4953ff",
          "name": "getJob",
          "request": {
            "url": "http://example.com/api/?Action=GetJob?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56c62501-bd90-438a-b9a0-368a17de7fa1"
            }
          ]
        },
        {
          "id": "2c4f4d2f-c3a5-40ae-ac12-409079068950",
          "name": "listJobs",
          "request": {
            "url": "http://example.com/api/?Action=ListJobs?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ea6e594-f9fe-4781-b4ef-c597bf484a46"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Status",
      "item": [
        {
          "id": "1569d758-337a-47e1-966e-f8fd907ace9d",
          "name": "getOfferingStatus",
          "request": {
            "url": "http://example.com/api/?Action=GetOfferingStatus?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the current status and future status of all offerings purchased by an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "880009a8-0275-4baa-81aa-183d3aa119ac"
            }
          ]
        }
      ]
    },
    {
      "name": "Suites",
      "item": [
        {
          "id": "df2b80f6-f292-4c8e-89b1-ff332a58be4c",
          "name": "getSuite",
          "request": {
            "url": "http://example.com/api/?Action=GetSuite?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a suite."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5cb3839-c832-43ae-9834-86303ede49b9"
            }
          ]
        },
        {
          "id": "3a08b168-50c6-4043-b735-f7af0f3c8e82",
          "name": "listSuites",
          "request": {
            "url": "http://example.com/api/?Action=ListSuites?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about suites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7a325c8-86c6-4421-afcf-77de382715a4"
            }
          ]
        }
      ]
    },
    {
      "name": "Tests",
      "item": [
        {
          "id": "21f0f7ba-95f0-4eaf-bc15-4502ad6ab4a7",
          "name": "getTest",
          "request": {
            "url": "http://example.com/api/?Action=GetTest?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about a test."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ce5459e-c9c9-4241-8669-74b4dcce3e55"
            }
          ]
        },
        {
          "id": "c816db3f-e15d-4294-b7fd-d8f1b8baa71d",
          "name": "listTests",
          "request": {
            "url": "http://example.com/api/?Action=ListTests?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about tests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9da9627e-701b-4a69-80aa-c1fe5734564c"
            }
          ]
        }
      ]
    },
    {
      "name": "Artifacts",
      "item": [
        {
          "id": "b5ae21b5-4b1a-477f-b7ca-41a51f5975da",
          "name": "listArtifacts",
          "request": {
            "url": "http://example.com/api/?Action=ListArtifacts?arn=arn&nextToken=nextToken&type=type",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about artifacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cefcd4f-3cf1-4a37-9879-f0e040478d6f"
            }
          ]
        }
      ]
    },
    {
      "name": "Offerings",
      "item": [
        {
          "id": "39c9f900-47a9-4c3c-83cf-1044136ade69",
          "name": "listOfferings",
          "request": {
            "url": "http://example.com/api/?Action=ListOfferings?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of products or offerings that the user can manage through the API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9f99725-1ad3-4ef6-9411-49fce3d8d918"
            }
          ]
        },
        {
          "id": "90e351ab-3424-4788-8f5b-4101d785b69a",
          "name": "purchaseOffering",
          "request": {
            "url": "http://example.com/api/?Action=PurchaseOffering?offeringId=offeringId&quantity=quantity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Immediately purchases offerings for an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "617fdc17-3966-425e-9f28-3dd157a77751"
            }
          ]
        },
        {
          "id": "20762758-dc83-4cbd-9547-a90eb4eb6aab",
          "name": "renewOffering",
          "request": {
            "url": "http://example.com/api/?Action=RenewOffering?offeringId=offeringId&quantity=quantity",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Explicitly sets the quantity of devices to renew for an offering, starting from the\n      effectiveDate of the next period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abf2c666-d798-40e3-94ab-3e46f16d6562"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Transactions",
      "item": [
        {
          "id": "2a01f338-fde5-475b-bf30-17c15ae63864",
          "name": "listOfferingTransactions",
          "request": {
            "url": "http://example.com/api/?Action=ListOfferingTransactions?nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of all historical purchases, renewals, and system renewal transactions for an\n      AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6cffaa0e-f5bb-4c0b-a11f-97225747a013"
            }
          ]
        }
      ]
    },
    {
      "name": "Samples",
      "item": [
        {
          "id": "6b8b7cd8-5488-4c67-a6e0-78e272e2d7ef",
          "name": "listSamples",
          "request": {
            "url": "http://example.com/api/?Action=ListSamples?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about samples, given an AWS Device Farm project ARN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d92462f-644b-469c-bd20-e540fb2b9f45"
            }
          ]
        }
      ]
    },
    {
      "name": "Unique Problems",
      "item": [
        {
          "id": "4cc76033-5a43-4174-8440-1a5238f0f2d7",
          "name": "listUniqueProblems",
          "request": {
            "url": "http://example.com/api/?Action=ListUniqueProblems?arn=arn&nextToken=nextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about unique problems."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2378a4ff-af8f-4ff8-9ed9-87cf5c258407"
            }
          ]
        }
      ]
    }
  ]
}