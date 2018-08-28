---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API List incoming webhooks
  description: |-
    Get a page of a list of incoming webhooks. Optionally filter for a specific team using query parameters.
    ##### Permissions
    `manage_webhooks` for the system or `manage_webhooks` for the specific team.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /hooks/incoming:
    get:
      summary: List incoming webhooks
      description: |-
        Get a page of a list of incoming webhooks. Optionally filter for a specific team using query parameters.
        ##### Permissions
        `manage_webhooks` for the system or `manage_webhooks` for the specific team.
      operationId: get-a-page-of-a-list-of-incoming-webhooks-optionally-filter-for-a-specific-team-using-query-paramete
      x-api-path-slug: hooksincoming-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of hooks per page
      - in: query
        name: team_id
        description: The ID of the team to get hooks for
      responses:
        200:
          description: OK
      tags:
      - List
      - Incoming
      - Webhooks
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