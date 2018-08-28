---
swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 0
info:
  title: AWS Auto Scaling API Describe Lifecycle Hooks
  version: 1.0.0
  description: Describes the lifecycle hooks for the specified Auto Scaling group.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeLifecycleHooks:
    get:
      summary: Describe Lifecycle Hooks
      description: Describes the lifecycle hooks for the specified Auto Scaling group.
      operationId: describeLifecycleHooks
      x-api-path-slug: actiondescribelifecyclehooks-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the group
        type: string
      - in: query
        name: LifecycleHookNames.member.N
        description: The names of one or more lifecycle hooks
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
  /?Action=DeleteLifecycleHook:
    get:
      summary: Delete Lifecycle Hook
      description: Deletes the specified lifecycle hook.
      operationId: deleteLifecycleHook
      x-api-path-slug: actiondeletelifecyclehook-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group for the lifecycle hook
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
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