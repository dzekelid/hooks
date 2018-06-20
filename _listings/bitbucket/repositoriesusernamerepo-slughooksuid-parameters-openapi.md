---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Repositories Username Repo Slug Hooks U
  description: Parameters repositories username repo slug hooks u
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repositories/{username}/{repo_slug}/hooks:
    get:
      summary: Get Repositories Username Repo Slug Hooks
      description: Returns a paginated list of webhooks installed on this repository.
      operationId: getRepositoriesUsernameRepoSlugHooks
      x-api-path-slug: repositoriesusernamerepo-slughooks-get
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Hooks
    parameters:
      summary: Parameters Repositories Username Repo Slug Hooks
      description: Parameters repositories username repo slug hooks
      operationId: parametersRepositoriesUsernameRepoSlugHooks
      x-api-path-slug: repositoriesusernamerepo-slughooks-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Hooks
    post:
      summary: Add Repositories Username Repo Slug Hooks
      description: |-
        Creates a new webhook on the specified repository.

        Example:

        ```
        $ curl -X POST -u credentials -H 'Content-Type: application/json'           https://api.bitbucket.org/2.0/repositories/username/slug/hooks           -d '
            {
              "description": "Webhook Description",
              "url": "https://example.com/",
              "active": true,
              "events": [
                "repo:push",
                "issue:created",
                "issue:updated"
              ]
            }'
        ```

        Note that this call requires the webhook scope, as well as any scope
        that applies to the events that the webhook subscribes to. In the
        example above that means: `webhook`, `repository` and `issue`.

        Also note that the `url` must properly resolve and cannot be an
        internal, non-routed address.
      operationId: postRepositoriesUsernameRepoSlugHooks
      x-api-path-slug: repositoriesusernamerepo-slughooks-post
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Hooks
  /repositories/{username}/{repo_slug}/hooks/{uid}:
    delete:
      summary: Delete Repositories Username Repo Slug Hooks U
      description: |-
        Deletes the specified webhook subscription from the given
        repository.
      operationId: deleteRepositoriesUsernameRepoSlugHooksU
      x-api-path-slug: repositoriesusernamerepo-slughooksuid-delete
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Hooks
      - U
    get:
      summary: Get Repositories Username Repo Slug Hooks U
      description: |-
        Returns the webhook with the specified id installed on the specified
        repository.
      operationId: getRepositoriesUsernameRepoSlugHooksU
      x-api-path-slug: repositoriesusernamerepo-slughooksuid-get
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Hooks
      - U
    parameters:
      summary: Parameters Repositories Username Repo Slug Hooks U
      description: Parameters repositories username repo slug hooks u
      operationId: parametersRepositoriesUsernameRepoSlugHooksU
      x-api-path-slug: repositoriesusernamerepo-slughooksuid-parameters
      responses:
        200:
          description: OK
      tags:
      - Repositories
      - Username
      - Repo
      - Slug
      - Hooks
      - U
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