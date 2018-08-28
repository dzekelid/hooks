---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 0
info:
  title: Bitbucket Parameters Hook Events Subject Type
  description: Parameters hook events subject type
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
    put:
      summary: Update Repositories Username Repo Slug Hooks U
      description: |-
        Updates the specified webhook subscription.

        The following properties can be mutated:

        * `description`
        * `url`
        * `active`
        * `events`
      operationId: putRepositoriesUsernameRepoSlugHooksU
      x-api-path-slug: repositoriesusernamerepo-slughooksuid-put
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
  /teams/{username}/hooks:
    get:
      summary: Get Teams Username Hooks
      description: Returns a paginated list of webhooks installed on this team.
      operationId: getTeamsUsernameHooks
      x-api-path-slug: teamsusernamehooks-get
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Username
      - Hooks
    parameters:
      summary: Parameters Teams Username Hooks
      description: Parameters teams username hooks
      operationId: parametersTeamsUsernameHooks
      x-api-path-slug: teamsusernamehooks-parameters
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Username
      - Hooks
    post:
      summary: Add Teams Username Hooks
      description: |-
        Creates a new webhook on the specified team.

        Team webhooks are fired for events from all repositories belonging to
        that team account.

        Note that only admins can install webhooks on teams.
      operationId: postTeamsUsernameHooks
      x-api-path-slug: teamsusernamehooks-post
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Username
      - Hooks
  /teams/{username}/hooks/{uid}:
    delete:
      summary: Delete Teams Username Hooks U
      description: |-
        Deletes the specified webhook subscription from the given team
        account.
      operationId: deleteTeamsUsernameHooksU
      x-api-path-slug: teamsusernamehooksuid-delete
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Username
      - Hooks
      - U
    get:
      summary: Get Teams Username Hooks U
      description: |-
        Returns the webhook with the specified id installed on the given
        team account.
      operationId: getTeamsUsernameHooksU
      x-api-path-slug: teamsusernamehooksuid-get
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Username
      - Hooks
      - U
    parameters:
      summary: Parameters Teams Username Hooks U
      description: Parameters teams username hooks u
      operationId: parametersTeamsUsernameHooksU
      x-api-path-slug: teamsusernamehooksuid-parameters
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Username
      - Hooks
      - U
    put:
      summary: Update Teams Username Hooks U
      description: |-
        Updates the specified webhook subscription.

        The following properties can be mutated:

        * `description`
        * `url`
        * `active`
        * `events`
      operationId: putTeamsUsernameHooksU
      x-api-path-slug: teamsusernamehooksuid-put
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Teams
      - Username
      - Hooks
      - U
  /users/{username}/hooks:
    get:
      summary: Get Users Username Hooks
      description: Returns a paginated list of webhooks installed on this user account.
      operationId: getUsersUsernameHooks
      x-api-path-slug: usersusernamehooks-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
    parameters:
      summary: Parameters Users Username Hooks
      description: Parameters users username hooks
      operationId: parametersUsersUsernameHooks
      x-api-path-slug: usersusernamehooks-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
    post:
      summary: Add Users Username Hooks
      description: |-
        Creates a new webhook on the specified user account.

        Account-level webhooks are fired for events from all repositories
        belonging to that account.

        Note that one can only register webhooks on one's own account, not that
        of others.
      operationId: postUsersUsernameHooks
      x-api-path-slug: usersusernamehooks-post
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
  /users/{username}/hooks/{uid}:
    delete:
      summary: Delete Users Username Hooks U
      description: |-
        Deletes the specified webhook subscription from the given user
        account.
      operationId: deleteUsersUsernameHooksU
      x-api-path-slug: usersusernamehooksuid-delete
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
      - U
    get:
      summary: Get Users Username Hooks U
      description: |-
        Returns the webhook with the specified id installed on the given
        user account.
      operationId: getUsersUsernameHooksU
      x-api-path-slug: usersusernamehooksuid-get
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
      - U
    parameters:
      summary: Parameters Users Username Hooks U
      description: Parameters users username hooks u
      operationId: parametersUsersUsernameHooksU
      x-api-path-slug: usersusernamehooksuid-parameters
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
      - U
    put:
      summary: Update Users Username Hooks U
      description: |-
        Updates the specified webhook subscription.

        The following properties can be mutated:

        * `description`
        * `url`
        * `active`
        * `events`
      operationId: putUsersUsernameHooksU
      x-api-path-slug: usersusernamehooksuid-put
      parameters:
      - in: path
        name: uid
        description: The installed webhooks id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Hooks
      - U
  /hook_events:
    get:
      summary: Get Hook Events
      description: |-
        Returns the webhook resource or subject types on which webhooks can
        be registered.

        Each resource/subject type contains an `events` link that returns the
        paginated list of specific events each individual subject type can
        emit.

        This endpoint is publicly accessible and does not require
        authentication or scopes.

        Example:

        ```
        $ curl https://api.bitbucket.org/2.0/hook_events

        {
            "repository": {
                "links": {
                    "events": {
                        "href": "https://api.bitbucket.org/2.0/hook_events/repository"
                    }
                }
            },
            "team": {
                "links": {
                    "events": {
                        "href": "https://api.bitbucket.org/2.0/hook_events/team"
                    }
                }
            },
            "user": {
                "links": {
                    "events": {
                        "href": "https://api.bitbucket.org/2.0/hook_events/user"
                    }
                }
            }
        }
        ```
      operationId: getHookEvents
      x-api-path-slug: hook-events-get
      responses:
        200:
          description: OK
      tags:
      - Hook
      - Events
    parameters:
      summary: Parameters Hook Events
      description: Parameters hook events
      operationId: parametersHookEvents
      x-api-path-slug: hook-events-parameters
      responses:
        200:
          description: OK
      tags:
      - Hook
      - Events
  /hook_events/{subject_type}:
    get:
      summary: Get Hook Events Subject Type
      description: |-
        Returns a paginated list of all valid webhook events for the
        specified entity.

        This is public data that does not require any scopes or authentication.

        Example:

        NOTE: The following example is a truncated response object for the `team` `subject_type`.
        We return the same structure for the other `subject_type` objects.

        ```
        $ curl https://api.bitbucket.org/2.0/hook_events/team
        {
            "page": 1,
            "pagelen": 30,
            "size": 21,
            "values": [
                {
                    "category": "Repository",
                    "description": "Whenever a repository push occurs",
                    "event": "repo:push",
                    "label": "Push"
                },
                {
                    "category": "Repository",
                    "description": "Whenever a repository fork occurs",
                    "event": "repo:fork",
                    "label": "Fork"
                },
                ...
                {
                    "category": "Repository",
                    "description": "Whenever a repository import occurs",
                    "event": "repo:imported",
                    "label": "Import"
                }
            ]
        }
        ```
      operationId: getHookEventsSubjectType
      x-api-path-slug: hook-eventssubject-type-get
      parameters:
      - in: path
        name: subject_type
        description: A resource or subject type
      responses:
        200:
          description: OK
      tags:
      - Hook
      - Events
      - Subject
      - Type
    parameters:
      summary: Parameters Hook Events Subject Type
      description: Parameters hook events subject type
      operationId: parametersHookEventsSubjectType
      x-api-path-slug: hook-eventssubject-type-parameters
      responses:
        200:
          description: OK
      tags:
      - Hook
      - Events
      - Subject
      - Type
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