---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Hooks
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket - Get Repositories Username Repo Slug Hooks
  x-api-slug: repositoriesusernamerepo-slughooks-get
  description: Returns a paginated list of webhooks installed on this repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Hooks
  x-api-slug: repositoriesusernamerepo-slughooks-parameters
  description: Parameters repositories username repo slug hooks
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-parameters-openapi.md
- name: Bitbucket - Add Repositories Username Repo Slug Hooks
  x-api-slug: repositoriesusernamerepo-slughooks-post
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooks-post-openapi.md
- name: Bitbucket - Delete Repositories Username Repo Slug Hooks U
  x-api-slug: repositoriesusernamerepo-slughooksuid-delete
  description: |-
    Deletes the specified webhook subscription from the given
    repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-delete-openapi.md
- name: Bitbucket - Get Repositories Username Repo Slug Hooks U
  x-api-slug: repositoriesusernamerepo-slughooksuid-get
  description: |-
    Returns the webhook with the specified id installed on the specified
    repository.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-get-openapi.md
- name: Bitbucket - Parameters Repositories Username Repo Slug Hooks U
  x-api-slug: repositoriesusernamerepo-slughooksuid-parameters
  description: Parameters repositories username repo slug hooks u
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-parameters-openapi.md
- name: Bitbucket - Update Repositories Username Repo Slug Hooks U
  x-api-slug: repositoriesusernamerepo-slughooksuid-put
  description: |-
    Updates the specified webhook subscription.

    The following properties can be mutated:

    * `description`
    * `url`
    * `active`
    * `events`
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/repositoriesusernamerepo-slughooksuid-put-openapi.md
- name: Bitbucket - Get Teams Username Hooks
  x-api-slug: teamsusernamehooks-get
  description: Returns a paginated list of webhooks installed on this team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooks-get-openapi.md
- name: Bitbucket - Parameters Teams Username Hooks
  x-api-slug: teamsusernamehooks-parameters
  description: Parameters teams username hooks
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooks-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooks-parameters-openapi.md
- name: Bitbucket - Add Teams Username Hooks
  x-api-slug: teamsusernamehooks-post
  description: |-
    Creates a new webhook on the specified team.

    Team webhooks are fired for events from all repositories belonging to
    that team account.

    Note that only admins can install webhooks on teams.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooks-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooks-post-openapi.md
- name: Bitbucket - Delete Teams Username Hooks U
  x-api-slug: teamsusernamehooksuid-delete
  description: |-
    Deletes the specified webhook subscription from the given team
    account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooksuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooksuid-delete-openapi.md
- name: Bitbucket - Get Teams Username Hooks U
  x-api-slug: teamsusernamehooksuid-get
  description: |-
    Returns the webhook with the specified id installed on the given
    team account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooksuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooksuid-get-openapi.md
- name: Bitbucket - Parameters Teams Username Hooks U
  x-api-slug: teamsusernamehooksuid-parameters
  description: Parameters teams username hooks u
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooksuid-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooksuid-parameters-openapi.md
- name: Bitbucket - Update Teams Username Hooks U
  x-api-slug: teamsusernamehooksuid-put
  description: |-
    Updates the specified webhook subscription.

    The following properties can be mutated:

    * `description`
    * `url`
    * `active`
    * `events`
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooksuid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/teamsusernamehooksuid-put-openapi.md
- name: Bitbucket - Get Users Username Hooks
  x-api-slug: usersusernamehooks-get
  description: Returns a paginated list of webhooks installed on this user account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooks-get-openapi.md
- name: Bitbucket - Parameters Users Username Hooks
  x-api-slug: usersusernamehooks-parameters
  description: Parameters users username hooks
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooks-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooks-parameters-openapi.md
- name: Bitbucket - Add Users Username Hooks
  x-api-slug: usersusernamehooks-post
  description: |-
    Creates a new webhook on the specified user account.

    Account-level webhooks are fired for events from all repositories
    belonging to that account.

    Note that one can only register webhooks on one's own account, not that
    of others.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooks-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooks-post-openapi.md
- name: Bitbucket - Delete Users Username Hooks U
  x-api-slug: usersusernamehooksuid-delete
  description: |-
    Deletes the specified webhook subscription from the given user
    account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooksuid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooksuid-delete-openapi.md
- name: Bitbucket - Get Users Username Hooks U
  x-api-slug: usersusernamehooksuid-get
  description: |-
    Returns the webhook with the specified id installed on the given
    user account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooksuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooksuid-get-openapi.md
- name: Bitbucket - Parameters Users Username Hooks U
  x-api-slug: usersusernamehooksuid-parameters
  description: Parameters users username hooks u
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooksuid-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooksuid-parameters-openapi.md
- name: Bitbucket - Update Users Username Hooks U
  x-api-slug: usersusernamehooksuid-put
  description: |-
    Updates the specified webhook subscription.

    The following properties can be mutated:

    * `description`
    * `url`
    * `active`
    * `events`
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooksuid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/usersusernamehooksuid-put-openapi.md
- name: Bitbucket - Get Hook Events
  x-api-slug: hook-events-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-events-get-openapi.md
- name: Bitbucket - Parameters Hook Events
  x-api-slug: hook-events-parameters
  description: Parameters hook events
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-events-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-events-parameters-openapi.md
- name: Bitbucket - Get Hook Events Subject Type
  x-api-slug: hook-eventssubject-type-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-eventssubject-type-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-eventssubject-type-get-openapi.md
- name: Bitbucket - Parameters Hook Events Subject Type
  x-api-slug: hook-eventssubject-type-parameters
  description: Parameters hook events subject type
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-eventssubject-type-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-eventssubject-type-parameters-openapi.md
- name: Bitbucket - Parameters Hook Events Subject Type
  x-api-slug: hook-eventssubject-type-parameters
  description: Parameters hook events subject type
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-eventssubject-type-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-eventssubject-type-parameters-openapi.md
- name: Bitbucket - Get Hook Events Subject Type
  x-api-slug: hook-eventssubject-type-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-eventssubject-type-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-eventssubject-type-get-openapi.md
- name: Bitbucket - Parameters Hook Events
  x-api-slug: hook-events-parameters
  description: Parameters hook events
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-events-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-events-parameters-openapi.md
- name: Bitbucket - Get Hook Events
  x-api-slug: hook-events-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Imports, Stack Network, Developers, Code, Technology, SaaS, Enterprise, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/hooks/master/_listings/bitbucket/hook-events-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://bigoven.api.gallery.streamdata.io
- type: x-api-stack
  url: http://bitbucket.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---