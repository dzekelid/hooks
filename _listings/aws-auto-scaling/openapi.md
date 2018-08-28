swagger: "2.0"
x-collection-name: AWS Auto Scaling
x-complete: 1
info:
  title: AWS Auto Scaling API
  version: 1.0.0
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
  /?Action=DescribeLifecycleHookTypes:
    get:
      summary: Describe Lifecycle Hook Types
      description: Describes the available types of lifecycle hooks.
      operationId: describeLifecycleHookTypes
      x-api-path-slug: actiondescribelifecyclehooktypes-get
      parameters:
      - in: query
        name: LifecycleHookTypes.member.N
        description: The lifecycle hook types
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle
  /?Action=PutLifecycleHook:
    get:
      summary: Put Lifecycle Hook
      description: Creates or updates a lifecycle hook for the specified Auto Scaling
        Group.
      operationId: putLifecycleHook
      x-api-path-slug: actionputlifecyclehook-get
      parameters:
      - in: query
        name: AutoScalingGroupName
        description: The name of the Auto Scaling group to which you want to assign
          the lifecycle hook
        type: string
      - in: query
        name: DefaultResult
        description: Defines the action the Auto Scaling group should take when the
          lifecycle hook timeout elapses or if an unexpected failure occurs
        type: string
      - in: query
        name: HeartbeatTimeout
        description: The amount of time, in seconds, that can elapse before the lifecycle
          hook times out
        type: string
      - in: query
        name: LifecycleHookName
        description: The name of the lifecycle hook
        type: string
      - in: query
        name: LifecycleTransition
        description: The instance state to which you want to attach the lifecycle
          hook
        type: string
      - in: query
        name: NotificationMetadata
        description: Contains additional information that you want to include any
          time Auto Scaling sends a message to the notification target
        type: string
      - in: query
        name: NotificationTargetARN
        description: The ARN of the notification target that Auto Scaling will use
          to notify you when an instance is in the transition state for the lifecycle
          hook
        type: string
      - in: query
        name: RoleARN
        description: The ARN of the IAM role that allows the Auto Scaling group to
          publish to the specified notification target
        type: string
      responses:
        200:
          description: OK
      tags:
      - Life Cycle