---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Delete Hooks
  version: 1.0.0
  description: Delete a hook
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/hooks:
    get:
      summary: Get Projects Hooks
      description: Get projects hooks.
      operationId: getV3ProjectsIdHooks
      x-api-path-slug: v3projectsidhooks-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Hooks
    post:
      summary: Post Projects Hooks
      description: Post projects hooks.
      operationId: postV3ProjectsIdHooks
      x-api-path-slug: v3projectsidhooks-post
      parameters:
      - in: formData
        name: build_events
        description: Trigger hook on build events
      - in: formData
        name: enable_ssl_verification
        description: Do SSL verification when triggering the hook
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: issues_events
        description: Trigger hook on issues events
      - in: formData
        name: merge_requests_events
        description: Trigger hook on merge request events
      - in: formData
        name: note_events
        description: Trigger hook on note(comment) events
      - in: formData
        name: pipeline_events
        description: Trigger hook on pipeline events
      - in: formData
        name: push_events
        description: Trigger hook on push events
      - in: formData
        name: tag_push_events
        description: Trigger hook on tag push events
      - in: formData
        name: token
        description: Secret token to validate received payloads; this will not be
          returned in the response
      - in: formData
        name: url
        description: The URL to send the request to
      - in: formData
        name: wiki_page_events
        description: Trigger hook on wiki events
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Hooks
  /v3/projects/{id}/hooks/{hook_id}:
    get:
      summary: Get Projects Hooks Hook
      description: Get projects hooks hook.
      operationId: getV3ProjectsIdHooksHookId
      x-api-path-slug: v3projectsidhookshook-id-get
      parameters:
      - in: path
        name: hook_id
        description: The ID of a project hook
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Hooks
      - Hook
    put:
      summary: Put Projects Hooks Hook
      description: Update an existing project hook
      operationId: putV3ProjectsIdHooksHookId
      x-api-path-slug: v3projectsidhookshook-id-put
      parameters:
      - in: formData
        name: build_events
        description: Trigger hook on build events
      - in: formData
        name: enable_ssl_verification
        description: Do SSL verification when triggering the hook
      - in: path
        name: hook_id
        description: The ID of the hook to update
      - in: path
        name: id
        description: The ID of a project
      - in: formData
        name: issues_events
        description: Trigger hook on issues events
      - in: formData
        name: merge_requests_events
        description: Trigger hook on merge request events
      - in: formData
        name: note_events
        description: Trigger hook on note(comment) events
      - in: formData
        name: pipeline_events
        description: Trigger hook on pipeline events
      - in: formData
        name: push_events
        description: Trigger hook on push events
      - in: formData
        name: tag_push_events
        description: Trigger hook on tag push events
      - in: formData
        name: token
        description: Secret token to validate received payloads; this will not be
          returned in the response
      - in: formData
        name: url
        description: The URL to send the request to
      - in: formData
        name: wiki_page_events
        description: Trigger hook on wiki events
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Hooks
      - Hook
    delete:
      summary: Delete Projects Hooks Hook
      description: Delete projects hooks hook.
      operationId: deleteV3ProjectsIdHooksHookId
      x-api-path-slug: v3projectsidhookshook-id-delete
      parameters:
      - in: path
        name: hook_id
        description: The ID of the hook to delete
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Hooks
      - Hook
  /v3/hooks:
    get:
      summary: Get Hooks
      description: Get the list of system hooks
      operationId: getV3Hooks
      x-api-path-slug: v3hooks-get
      responses:
        200:
          description: OK
      tags:
      - Hooks
    post:
      summary: Post Hooks
      description: Create a new system hook
      operationId: postV3Hooks
      x-api-path-slug: v3hooks-post
      parameters:
      - in: formData
        name: enable_ssl_verification
        description: Do SSL verification when triggering the hook
      - in: formData
        name: push_events
        description: Trigger hook on push events
      - in: formData
        name: tag_push_events
        description: Trigger hook on tag push events
      - in: formData
        name: token
        description: The token used to validate payloads
      - in: formData
        name: url
        description: The URL to send the request to
      responses:
        200:
          description: OK
      tags:
      - Hooks
  /v3/hooks/{id}:
    get:
      summary: Get Hooks
      description: Test a hook
      operationId: getV3HooksId
      x-api-path-slug: v3hooksid-get
      parameters:
      - in: path
        name: id
        description: The ID of the system hook
      responses:
        200:
          description: OK
      tags:
      - Hooks
    delete:
      summary: Delete Hooks
      description: Delete a hook
      operationId: deleteV3HooksId
      x-api-path-slug: v3hooksid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the system hook
      responses:
        200:
          description: OK
      tags:
      - Hooks
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