{
  "info": {
    "name": "AWS Device Farm API List Runs",
    "_postman_id": "e8980179-7531-4a92-bc3c-fd0f46a4df11",
    "description": "Gets information about runs, given an AWS Device Farm project ARN.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device Pool",
      "item": [
        {
          "id": "35386ff4-c754-46b8-b2de-b051df5554a6",
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
              "id": "ac903c06-bca5-4726-a88c-948883ff7b26"
            }
          ]
        },
        {
          "id": "96ceb953-57db-4bce-9d36-8362e6ba0dbc",
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
              "id": "059a3b2d-5423-4768-ba1e-00c2fb4abde7"
            }
          ]
        },
        {
          "id": "1a5074e1-b335-4f81-9b42-bfe5103c7314",
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
              "id": "def047c0-1738-46f8-8cc0-a8ef4294a9fb"
            }
          ]
        },
        {
          "id": "57505b88-fd4e-42b0-bd6a-8e54ceba0bcc",
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
              "id": "3f6b05a9-b4a3-401f-b40e-9d7858b0b89b"
            }
          ]
        },
        {
          "id": "6b6a3a0c-ba00-4de1-b0e1-15288405481e",
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
              "id": "22ea1667-c0e7-41e7-987a-b61e99170e93"
            }
          ]
        }
      ]
    },
    {
      "name": "Project",
      "item": [
        {
          "id": "eebc2361-eb3b-441b-83d9-affb95b85201",
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
              "id": "8f58cd02-ac94-4c1c-bcff-f91074e2b492"
            }
          ]
        }
      ]
    },
    {
      "name": "Remote Access Sessions",
      "item": [
        {
          "id": "75bcf826-d345-4375-aa12-96cd8cacee54",
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
              "id": "7056cc78-791b-4391-9ef3-02f7fa385687"
            }
          ]
        },
        {
          "id": "225286ed-96ec-406d-8c02-cfc6f0d4b408",
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
              "id": "68a67663-db9d-4965-880a-be6fb80ed216"
            }
          ]
        },
        {
          "id": "d64ee9c4-6326-4802-8b6a-f5298af60728",
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
              "id": "b1e59b78-1cce-41eb-8df6-9d09acf22202"
            }
          ]
        },
        {
          "id": "f72ff58a-489d-490d-a922-63c4d890cee0",
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
              "id": "bafd22f5-00ab-4117-adf4-b50524682994"
            }
          ]
        },
        {
          "id": "8f1f9abf-be77-490c-9421-089220bd62ae",
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
              "id": "f75b7d94-986a-4b0a-9bd8-961c225db291"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "820740e6-9023-47c3-99fd-22cb11b54513",
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
              "id": "787ee3e7-ca64-407a-9875-00e650c9e5c8"
            }
          ]
        },
        {
          "id": "7535be87-7ea7-4efd-8b07-865ea896287f",
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
              "id": "0b2dbba1-a0a4-44d9-a49f-72a60f81c48f"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "4f105d20-e895-4397-be8a-8b05596e9977",
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
              "id": "a8094b44-7904-4f1e-abca-2ee01a6634e4"
            }
          ]
        },
        {
          "id": "47d097b4-866d-45a0-ae59-d45196469788",
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
              "id": "f770858d-e567-4945-9c7f-fbf617a0af4c"
            }
          ]
        },
        {
          "id": "88fd5bc6-cf01-4f84-9152-aa1b39a74afd",
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
              "id": "f55bc8f1-198c-4595-bf91-e2c9d0dad3b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Runs",
      "item": [
        {
          "id": "8ffeca5a-3b93-408b-bcd2-29d2c949c3e5",
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
              "id": "55659782-4cca-4806-9d4a-140d6ad19d63"
            }
          ]
        },
        {
          "id": "f89daa83-f86c-4bbf-b257-46b7535f746d",
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
              "id": "f858d67e-0800-43b8-a02a-40b3ff0726d7"
            }
          ]
        },
        {
          "id": "db5a9bc7-f407-4d6a-9001-aa64d040cb5f",
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
              "id": "879db1c2-a67f-4569-b76b-b25ac79e590c"
            }
          ]
        }
      ]
    },
    {
      "name": "Uploads",
      "item": [
        {
          "id": "8b5f9233-c0f4-4022-b059-7167b8be5ec0",
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
              "id": "54cd7449-4184-4077-a127-a936153c4af8"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Settings",
      "item": [
        {
          "id": "7bfa8a3d-1c01-4c79-85b9-50a4ffea452e",
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
              "id": "2dedfc0a-fcec-4980-a333-4dad1aa42378"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "5033ea3b-35f3-4166-a229-fb1248bc40dc",
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
              "id": "2c5f8ef9-cd6f-4e78-871d-6fe4ac18f8d5"
            }
          ]
        },
        {
          "id": "4513c48d-1afe-4b0f-a862-38a181331027",
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
              "id": "2c457634-588a-422d-b155-af5f37d72540"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "dee06c13-cb4e-4d5c-9a7e-a061d5efa10a",
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
              "id": "466aa5da-73e1-4a35-b19f-ea1aefe9f47d"
            }
          ]
        },
        {
          "id": "d6993941-b434-4713-9b16-bfa639aca5f0",
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
              "id": "2d250d17-d0da-46dd-8b52-38a83961ac6f"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Status",
      "item": [
        {
          "id": "2972c0f7-dd83-44d2-b1c7-1cbf661dbfab",
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
              "id": "9ca29749-ac3f-4255-9ed9-a7a93fca37e3"
            }
          ]
        }
      ]
    },
    {
      "name": "Suites",
      "item": [
        {
          "id": "df1e4f08-a2ce-44f4-b1ce-724c4be5df07",
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
              "id": "7a3a7809-0e6a-46d5-b655-a04ec44a8435"
            }
          ]
        }
      ]
    },
    {
      "name": "Tests",
      "item": [
        {
          "id": "516af345-9b68-441c-a246-3bca3f9254b9",
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
              "id": "9d3ce2e2-6992-451b-96d5-9ddd736886ff"
            }
          ]
        }
      ]
    },
    {
      "name": "Artifacts",
      "item": [
        {
          "id": "6d8e6b66-8d43-490d-b34e-df4d23b56570",
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
              "id": "fe2c591a-a4f8-4c66-b0be-478ff77bc286"
            }
          ]
        }
      ]
    },
    {
      "name": "Offerings",
      "item": [
        {
          "id": "f5d42bf6-97e7-4228-8830-8b76371f04c7",
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
              "id": "535c5028-78bc-426a-aeab-0ba6855c3ea1"
            }
          ]
        }
      ]
    },
    {
      "name": "Offering Transactions",
      "item": [
        {
          "id": "240783d6-cafb-4da8-955c-da70d7b7e23b",
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
              "id": "d43eb1a7-5915-4784-b695-d55527bcab5b"
            }
          ]
        }
      ]
    }
  ]
}