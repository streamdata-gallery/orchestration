---
swagger: "2.0"
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateLayer&k=1:
    get:
      summary: ' Create Layer '
      description: Creates a layer
      operationId: createLayer
      parameters:
      - in: query
        name: Attributes
        description: One or more user-defined key-value pairs to be added to the stack
          attributes
        type: string
      - in: query
        name: AutoAssignElasticIps
        description: Whether to automatically assign an Elastic IP        address
          to the layer's instances
        type: string
      - in: query
        name: AutoAssignPublicIps
        description: For stacks that are running in a VPC, whether to automatically
          assign a public IP address to      the layer's instances
        type: string
      - in: query
        name: CustomInstanceProfileArn
        description: The ARN of an IAM profile to be used for the layer's EC2 instances
        type: string
      - in: query
        name: CustomJson
        description: A JSON-formatted string containing custom stack configuration
          and deployment attributes     to be installed on the layer's instances
        type: string
      - in: query
        name: CustomRecipes
        description: A LayerCustomRecipes object that specifies the layer custom recipes
        type: string
      - in: query
        name: CustomSecurityGroupIds
        description: An array containing the layer custom security group IDs
        type: string
      - in: query
        name: EnableAutoHealing
        description: Whether to disable auto healing for the layer
        type: string
      - in: query
        name: InstallUpdatesOnBoot
        description: Whether to install operating system and package updates when
          the instance boots
        type: string
      - in: query
        name: LifecycleEventConfiguration
        description: A LifeCycleEventConfiguration object that you can use to configure
          the Shutdown event to      specify an execution timeout and enable or disable
          Elastic Load Balancer connection      draining
        type: string
      - in: query
        name: Name
        description: The layer name, which is used by the console
        type: string
      - in: query
        name: Packages
        description: An array of Package objects that describes the layer packages
        type: string
      - in: query
        name: Shortname
        description: For custom layers only, use this parameter to specify the layer's
          short name, which is used internally by AWS OpsWorks Stacks and by Chef
          recipes
        type: string
      - in: query
        name: StackId
        description: The layer stack ID
        type: string
      - in: query
        name: Type
        description: The layer type
        type: string
      - in: query
        name: UseEbsOptimizedInstances
        description: Whether to use Amazon EBS-optimized instances
        type: string
      - in: query
        name: VolumeConfigurations
        description: A VolumeConfigurations object that describes the layer's Amazon
          EBS volumes
        type: string
      responses:
        200:
          description: OK
      tags:
      - ""
definitions: []
x-collection-name: AWS OpsWorks
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