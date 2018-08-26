---
swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 1
info:
  title: AWS CodeDeploy API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=UpdateApplication:
    get:
      summary: Update Application
      description: Changes the name of an application.
      operationId: updateApplication
      x-api-path-slug: actionupdateapplication-get
      parameters:
      - in: query
        name: applicationName
        description: The current name of the application you want to change
        type: string
      - in: query
        name: newApplicationName
        description: The new name to give the application
        type: string
      responses:
        200:
          description: OK
      tags:
      - Applications
  /?Action=UpdateDeploymentGroup:
    get:
      summary: Update Deployment Group
      description: Changes information about a deployment group.
      operationId: updateDeploymentGroup
      x-api-path-slug: actionupdatedeploymentgroup-get
      parameters:
      - in: query
        name: alarmConfiguration
        description: Information to add or change about Amazon CloudWatch alarms when
          the deployment            group is updated
        type: string
      - in: query
        name: applicationName
        description: The application name corresponding to the deployment group to
          update
        type: string
      - in: query
        name: autoRollbackConfiguration
        description: Information for an automatic rollback configuration that is added
          or changed when a            deployment group is updated
        type: string
      - in: query
        name: autoScalingGroups
        description: The replacement list of Auto Scaling groups to be included in
          the deployment group,            if you want to change them
        type: string
      - in: query
        name: currentDeploymentGroupName
        description: The current name of the deployment group
        type: string
      - in: query
        name: deploymentConfigName
        description: The replacement deployment configuration name to use, if you
          want to change            it
        type: string
      - in: query
        name: ec2TagFilters
        description: The replacement set of Amazon EC2 tags on which to filter, if
          you want to change            them
        type: string
      - in: query
        name: newDeploymentGroupName
        description: The new name of the deployment group, if you want to change it
        type: string
      - in: query
        name: onPremisesInstanceTagFilters
        description: The replacement set of on-premises instance tags on which to
          filter, if you want to            change them
        type: string
      - in: query
        name: serviceRoleArn
        description: A replacement ARN for the service role, if you want to change
          it
        type: string
      - in: query
        name: triggerConfigurations
        description: Information about triggers to change when the deployment group
          is updated
        type: string
      responses:
        200:
          description: OK
      tags:
      - Deployment Groups
---