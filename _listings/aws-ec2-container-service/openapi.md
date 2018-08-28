swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 1
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateService:
    get:
      summary: Create Service
      description: Runs and maintains a desired number of tasks from a specified task
        definition.
      operationId: createService
      x-api-path-slug: actioncreateservice-get
      parameters:
      - in: query
        name: clientToken
        description: Unique, case-sensitive identifier you provide to ensure the idempotency
          of the            request
        type: string
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          on which to run your service
        type: string
      - in: query
        name: deploymentConfiguration
        description: Optional deployment parameters that control how many tasks run
          during the            deployment and the ordering of stopping and starting
          tasks
        type: string
      - in: query
        name: desiredCount
        description: The number of instantiations of the specified task definition
          to place and keep            running on your cluster
        type: string
      - in: query
        name: loadBalancers
        description: A load balancer object representing the load balancer to use
          with your service
        type: string
      - in: query
        name: placementConstraints
        description: An array of placement constraint objects to use for tasks in
          your service
        type: string
      - in: query
        name: placementStrategy
        description: The placement strategy objects to use for tasks in your service
        type: string
      - in: query
        name: role
        description: The name or full Amazon Resource Name (ARN) of the IAM role that
          allows Amazon ECS to make calls to your            load balancer on your
          behalf
        type: string
      - in: query
        name: serviceName
        description: The name of your service
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to run in your service
        type: string
      responses:
        200:
          description: OK
      tags:
      - Services
  /?Action=RunTask:
    get:
      summary: Run Task
      description: Starts a new task using the specified task definition.
      operationId: runTask
      x-api-path-slug: actionruntask-get
      parameters:
      - in: query
        name: cluster
        description: The short name or full Amazon Resource Name (ARN) of the cluster
          on which to run your task
        type: string
      - in: query
        name: count
        description: The number of instantiations of the specified task to place on
          your            cluster
        type: string
      - in: query
        name: group
        description: The name of the task group to associate with the task
        type: string
      - in: query
        name: overrides
        description: A list of container overrides in JSON format that specify the
          name of a container            in the specified task definition and the
          overrides it should receive
        type: string
      - in: query
        name: placementConstraints
        description: An array of placement constraint objects to use for the task
        type: string
      - in: query
        name: placementStrategy
        description: The placement strategy objects to use for the task
        type: string
      - in: query
        name: startedBy
        description: An optional tag specified when a task is started
        type: string
      - in: query
        name: taskDefinition
        description: The family and revision (family:revision) or            full
          Amazon Resource Name (ARN) of the task definition to run
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks