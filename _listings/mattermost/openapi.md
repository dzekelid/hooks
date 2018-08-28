---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-4-0-release--api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v5-0--details-heretagapiv3deprecation--looking-for-the-api-v3-reference-it-has-moved-herehttpsapi-mattermost-comv3-
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
  /hooks/outgoing:
    get:
      summary: List outgoing webhooks
      description: |-
        Get a page of a list of outgoing webhooks. Optionally filter for a specific team or channel using query parameters.
        ##### Permissions
        `manage_webhooks` for the system or `manage_webhooks` for the specific team/channel.
      operationId: get-a-page-of-a-list-of-outgoing-webhooks-optionally-filter-for-a-specific-team-or-channel-using-que
      x-api-path-slug: hooksoutgoing-get
      parameters:
      - in: query
        name: channel_id
        description: The ID of the channel to get hooks for
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
      - Outgoing
      - Webhooks
---