{
  "info": {
    "name": "AWS Device Farm API Stop Run",
    "_postman_id": "192bde03-c048-4fbf-bb3a-a622208d19d8",
    "description": "Initiates a stop request for the current test run.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "347c3b60-c09b-475f-a614-5eba2fb40128",
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
              "id": "617bd198-3108-480c-a543-acc0247eb1d4"
            }
          ]
        },
        {
          "id": "6fe7274b-6298-4c74-8dc8-64ccee74b23f",
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
              "id": "6b9685ae-da3b-4665-8809-30fce5d71d53"
            }
          ]
        },
        {
          "id": "a4ad0ed3-62d0-46a6-8683-230945a88c3c",
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
              "id": "bc9d531e-c587-462b-8c5f-688870c32374"
            }
          ]
        },
        {
          "id": "28910349-9286-4a62-8424-c18e5339b860",
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
              "id": "2367791e-fe68-4631-9c75-91d9b9afcafa"
            }
          ]
        },
        {
          "id": "671ac327-cc24-4fe8-bec0-cf6602116abf",
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
              "id": "2b00ae3e-0ec6-44ef-9c96-f2fdde5e1957"
            }
          ]
        }
      ]
    },
    {
      "name": "Project",
      "item": [
        {
          "id": "8ff1884e-5ef4-4b50-b8db-fe2ca1facb8f",
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
              "id": "62660d6f-9246-4276-b0a6-06ba8a1a7764"
            }
          ]
        }
      ]
    },
    {
      "name": "Remote Access Sessions",
      "item": [
        {
          "id": "df47a11d-d729-4e1e-8844-badc7e8e2964",
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
              "id": "db00e98f-95a6-4d9d-8e07-cf847933e04b"
            }
          ]
        },
        {
          "id": "79bf10c8-f39e-4f1b-a1b1-b65286651f60",
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
              "id": "982780a1-3683-458d-9d5d-e24a4a29ed74"
            }
          ]
        },
        {
          "id": "8e745724-774e-4517-b2e9-42daa0828392",
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
              "id": "772ded80-469e-41a8-a6c9-4528e0a566fb"
            }
          ]
        },
        {
          "id": "0f0c531e-6113-4b4c-bc7a-2e99e1ff42a0",
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
              "id": "7f684ce3-9898-4c50-a7b4-13fb06909835"
            }
          ]
        },
        {
          "id": "73598037-d7b3-4c34-99f2-1db2fc600220",
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
              "id": "acfff30e-a72e-4e0a-bf4c-559537a18a86"
            }
          ]
        },
        {
          "id": "0a444adc-e36b-4e86-ab3e-3982bbfaf2b7",
          "name": "stopRemoteAccessSession",
          "request": {
            "url": "http://example.com/api/?Action=StopRemoteAccessSession?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Ends a specified remote access session."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd4d3f14-f1a1-49ad-86cb-12cf064a9284"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "9ade0229-88a1-464b-96d9-e6a8f428d453",
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
              "id": "3ee3685e-4b35-4b52-ae47-e8fe8a00ad49"
            }
          ]
        },
        {
          "id": "d67d5a46-f9b4-44bb-a40e-c1df72e99542",
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
              "id": "c181841d-6c2a-448e-ac0e-ff98d75d4f69"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "f2ada8fc-5629-42f0-9582-4575308fe26b",
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
              "id": "70067dc3-c3bf-40dd-a247-7b427f6ca39b"
            }
          ]
        },
        {
          "id": "bd58dfef-537c-47cb-a31c-cba097253f77",
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
              "id": "6d1765fb-0339-495d-91e7-ccc949df43df"
            }
          ]
        },
        {
          "id": "8deb5d16-95d0-474e-9a9e-0066543de42e",
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
              "id": "a002d2f4-8435-42ee-9fa1-fc20029e9557"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "57405ac4-6ba0-48ca-b1aa-d562ff6a55d8",
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
              "id": "b79a6dab-8900-4812-94d4-a7f6e89c020d"
            }
          ]
        },
        {
          "id": "687aa6a9-7c2b-4a71-8107-359c2e5523fc",
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
              "id": "b20912cb-3b9e-4558-8a58-9facd7b47372"
            }
          ]
        },
        {
          "id": "b43e6ae6-05b0-45bf-b8af-ab48636f0e50",
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
              "id": "dd44e652-358a-431c-9bb4-32f97aee6c8c"
            }
          ]
        },
        {
          "id": "beea48a1-bf29-4b71-b340-33cf235a8ff7",
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
              "id": "5af04488-0a68-4457-9d39-3c44fe1301c0"
            }
          ]
        },
        {
          "id": "9e86cc24-d59e-4e56-9506-30cfa0531fc8",
          "name": "stopRun",
          "request": {
            "url": "http://example.com/api/?Action=StopRun?arn=arn",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates a stop request for the current test run."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a9d1e3a-cdfa-405f-9991-127a5ce7687a"
            }
          ]
        }
      ]
    },
    {
      "name": "Uploads",
      "item": [
        {
          "id": "1ab4857d-6813-4191-8931-9239d7c31cb1",
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
              "id": "c65736f7-5a41-41e9-875f-23ef3fccf909"
            }
          ]
        },
        {
          "id": "cde23030-9d3e-4c71-a04a-792a37177cdd",
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
              "id": "966ecf38-0747-411b-ac29-03576ec702cf"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Settings",
      "item": [
        {
          "id": "526ea315-7749-4cd3-8b60-15f07189d0de",
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
              "id": "db9b31b2-e2eb-4a75-90fe-97116ce13635"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "7786808b-605b-49e4-a60c-ff23c5fcb96d",
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
              "id": "4f2e69c3-04d8-492a-b7d5-fd7b9f2ba76e"
            }
          ]
        },
        {
          "id": "92c68e43-b6ea-4d12-bbc0-de373a00c51c",
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
              "id": "f957d869-2b06-46a2-be01-3c47070e830a"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "faa00a68-2af5-40f3-9e37-5eea2016379f",
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
              "id": "8b22ec58-2a61-491a-ae65-2d660bca610e"
            }
          ]
        },
        {
          "id": "8b282628-968e-4c72-8108-0bc009354a65",
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
              "id": "d2e29935-d29b-4ee4-9623-ef72208dce40"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Status",
      "item": [
        {
          "id": "8174d580-af12-49d9-8c73-d35926e9861c",
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
              "id": "0ecb27fc-1a1a-41ba-b042-bb4a967efda0"
            }
          ]
        }
      ]
    },
    {
      "name": "Suites",
      "item": [
        {
          "id": "6283713f-a9f5-4abf-8d10-fb1e4553a73f",
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
              "id": "671ad658-a79d-4231-8396-db651383fce7"
            }
          ]
        },
        {
          "id": "d82c3ff1-860c-4692-8a8a-42144d39fbf8",
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
              "id": "c95dad00-5401-42fe-859f-ca1a0c11d4a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Tests",
      "item": [
        {
          "id": "711dfbf5-7910-42a9-a0b2-cc4f244f27bf",
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
              "id": "3716038d-0e18-4b39-88c0-ba2213d79d4f"
            }
          ]
        },
        {
          "id": "d3025905-49c0-4cfc-a9c5-d186228b5053",
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
              "id": "0000ad3f-98a3-4449-b32d-cfb469051b41"
            }
          ]
        }
      ]
    },
    {
      "name": "Artifacts",
      "item": [
        {
          "id": "4e85ab0b-0fd8-4d2e-9fa4-5e77dbd4fb43",
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
              "id": "1df3cfaf-7d5d-4106-81a3-8f8c1a00b859"
            }
          ]
        }
      ]
    },
    {
      "name": "Offerings",
      "item": [
        {
          "id": "5968ffa8-48fe-4f11-aa6b-9b7c993c6f9a",
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
              "id": "5260a3fb-00c8-45f0-ae53-db16e22cc286"
            }
          ]
        },
        {
          "id": "f69f7b80-18c1-40cd-a61e-505bb0d3a292",
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
              "id": "6f8b0583-e759-4eec-a551-9fae5f99d495"
            }
          ]
        },
        {
          "id": "5913bc9c-7eeb-4989-9eb3-44e4d41255c7",
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
              "id": "e79de133-b881-4d13-a322-061dadf7882b"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Transactions",
      "item": [
        {
          "id": "c165b2f4-3282-4c74-9d13-d08409e41294",
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
              "id": "d047f36f-ef74-4f37-9675-ee2b734bb98d"
            }
          ]
        }
      ]
    },
    {
      "name": "Samples",
      "item": [
        {
          "id": "02537468-3d33-46db-8ce6-fce8cfc7effb",
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
              "id": "9a314652-79e0-45c4-88b7-3af6fa329f1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Unique Problems",
      "item": [
        {
          "id": "8b87f8f5-3fe5-4826-bcce-1b9cfbc2309e",
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
              "id": "b76d46b2-5133-4687-b830-5d6f532dae9a"
            }
          ]
        }
      ]
    }
  ]
}