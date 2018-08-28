---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Find user keys by query
  description: |-
    Finds users using a structured query and returns a list of user keys. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse users and groups_ [global permission](href=). The available query statements are:

    *   `is assignee of PROJ` Returns the users that are assignees of at least one issue in project _PROJ_.
    *   `is assignee of (PROJ-1, PROJ-2)` Returns users that are assignees on the issues _PROJ-1_ or _PROJ-2_.
    *   `is reporter of (PROJ-1, PROJ-2)` Returns users that are reporters on the issues _PROJ-1_ or _PROJ-2_.
    *   `is watcher of (PROJ-1, PROJ-2)` Returns users that are watchers on the issues _PROJ-1_ or _PROJ-2_.
    *   `is voter of (PROJ-1, PROJ-2)` Returns users that are voters on the issues _PROJ-1_ or _PROJ-2_.
    *   `is commenter of (PROJ-1, PROJ-2)` Returns users that have posted a comment on the issues _PROJ-1_ or _PROJ-2_.
    *   `is transitioner of (PROJ-1, PROJ-2)` Returns users that have performed a transition on issues _PROJ-1_ or _PROJ-2_.
    *   `[propertyKey].entity.property.path is "property value"` Returns users with the entity property value.

    The list of issues can be extended as needed, as in _(PROJ-1, PROJ-2, ... PROJ-n)_. Statements can be combined using the `AND` and `OR` operators to form more complex queries, for example:

    `is assignee of PROJ AND [propertyKey].entity.property.path is "property value"`
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /relation/{relationName}/from/{sourceType}/{sourceKey}/to/{targetType}:
    get:
      summary: Find target entities related to a source entity
      description: "Returns all target entities that have a particular relationship
        to the \nsource entity. Note, relationships are one way.\n\nFor example, the
        following method finds all content that the current user \nhas an 'ignore'
        relationship with:\n`GET https://your-domain.atlassian.net/wiki/rest/api/relation/ignore/from/user/current/to/content`\nNote,
        'ignore' is an example custom relationship type.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to view both the target entity and source entity."
      operationId: com.atlassian.confluence.plugins.restapi.resources.RelationResource.findTargetFromSource_get
      x-api-path-slug: relationrelationnamefromsourcetypesourcekeytotargettype-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the response
          object to expand
      - in: query
        name: limit
        description: The maximum number of relationships to return per page
      - in: path
        name: relationName
        description: The name of the relationship
      - in: path
        name: sourceKey
        description: '- The identifier for the source entity:- If `sourceType` is
          user, then specify either current (logged-in   user) or the user key'
      - in: query
        name: sourceStatus
        description: The status of the source
      - in: path
        name: sourceType
        description: The source entity type of the relationship
      - in: query
        name: sourceVersion
        description: The version of the source
      - in: query
        name: start
        description: The starting index of the returned relationships
      - in: query
        name: targetStatus
        description: The status of the target
      - in: path
        name: targetType
        description: The target entity type of the relationship
      - in: query
        name: targetVersion
        description: The version of the target
      responses:
        200:
          description: OK
      tags:
      - Find
      - Target
      - Entities
      - Related
      - To
      - Source
      - Entity
  /relation/{relationName}/from/{sourceType}/{sourceKey}/to/{targetType}/{targetKey}:
    get:
      summary: Find relationship from source to target
      description: "Find whether a particular type of relationship exists from a source
        \nentity to a target entity. Note, relationships are one way.\n\nFor example,
        you can use this method to find whether the current user has \nselected a
        particular page as a favorite (i.e. 'save for later'):\n`GET https://your-domain.atlassian.net/wiki/rest/api/relation/favourite/from/user/current/to/content/123`\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to view both the target entity and source entity."
      operationId: com.atlassian.confluence.plugins.restapi.resources.RelationResource.GetRelationship_get
      x-api-path-slug: relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the response
          object to expand
      - in: path
        name: relationName
        description: The name of the relationship
      - in: path
        name: sourceKey
        description: '- The identifier for the source entity:- If `sourceType` is
          user, then specify either current (logged-in   user) or the user key'
      - in: query
        name: sourceStatus
        description: The status of the source
      - in: path
        name: sourceType
        description: The source entity type of the relationship
      - in: query
        name: sourceVersion
        description: The version of the source
      - in: path
        name: targetKey
        description: '- The identifier for the target entity:- If `sourceType` is
          user, then specify either current (logged-in   user) or the user key'
      - in: query
        name: targetStatus
        description: The status of the target
      - in: path
        name: targetType
        description: The target entity type of the relationship
      - in: query
        name: targetVersion
        description: The version of the target
      responses:
        200:
          description: OK
      tags:
      - Find
      - Relationship
      - From
      - Source
      - To
      - Target
  /relation/{relationName}/to/{targetType}/{targetKey}/from/{sourceType}:
    get:
      summary: Find target entities related to a source entity
      description: "Returns all target entities that have a particular relationship
        to the \nsource entity. Note, relationships are one way.\n\nFor example, the
        following method finds all users that have a 'collaborator' \nrelationship
        to a piece of content with an ID of '1234':\n`GET https://your-domain.atlassian.net/wiki/rest/api/relation/collaborator/to/content/1234/from/user`\nNote,
        'collaborator' is an example custom relationship type.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \nPermission to view both the target entity and source entity."
      operationId: com.atlassian.confluence.plugins.restapi.resources.RelationResource.findSourcesForTarget_get
      x-api-path-slug: relationrelationnametotargettypetargetkeyfromsourcetype-get
      parameters:
      - in: query
        name: expand
        description: A multi-value parameter indicating which properties of the response
          object to expand
      - in: query
        name: limit
        description: The maximum number of relationships to return per page
      - in: path
        name: relationName
        description: The name of the relationship
      - in: query
        name: sourceStatus
        description: The status of the source
      - in: path
        name: sourceType
        description: The source entity type of the relationship
      - in: query
        name: sourceVersion
        description: The version of the source
      - in: query
        name: start
        description: The starting index of the returned relationships
      - in: path
        name: targetKey
        description: '- The identifier for the target entity:- If `sourceType` is
          user, then specify either current (logged-in   user) or the user key'
      - in: query
        name: targetStatus
        description: The status of the target
      - in: path
        name: targetType
        description: The target entity type of the relationship
      - in: query
        name: targetVersion
        description: The version of the target
      responses:
        200:
          description: OK
      tags:
      - Find
      - Target
      - Entities
      - Related
      - To
      - Source
      - Entity
  /api/2/groups/picker:
    get:
      summary: Find groups
      description: |-
        Returns groups with substrings matching a given query. This is mainly for use with the group picker, so the returned groups contain html to be used as picker suggestions. The groups are also wrapped in a single response object that also contains a header for use in the picker, specifically _Showing X of Y matching groups_.

        The number of groups returned is limited by the system property "jira.ajax.autocomplete.limit"

        The groups will be unique and sorted.
      operationId: com.atlassian.jira.rest.v2.issue.GroupPickerResource.findGroups_get
      x-api-path-slug: api2groupspicker-get
      parameters:
      - in: query
        name: accountId
      - in: query
        name: exclude
      - in: header
        name: force-account-id
      - in: query
        name: maxResults
      - in: query
        name: query
        description: a String to match groups agains
      - in: query
        name: userName
      responses:
        200:
          description: OK
      tags:
      - Find
      - Groups
  /api/2/groupuserpicker:
    get:
      summary: Find users and groups
      description: Returns a list of users and groups matching query with highlighting.
        This resource cannot be accessed anonymously.
      operationId: com.atlassian.jira.rest.v2.issue.GroupAndUserPickerResource.findUsersAndGroups_get
      x-api-path-slug: api2groupuserpicker-get
      parameters:
      - in: query
        name: avatarSize
        description: The size of the avatar to return
      - in: query
        name: caseInsensitive
        description: whether the search for groups should be case insensitive
      - in: query
        name: excludeConnectAddons
        description: Boolean indicating whether Connect Add-on users and groups should
          be excluded from the search results
      - in: query
        name: fieldId
        description: The custom field id, if this request comes from a custom field,
          such as a user picker
      - in: query
        name: issueTypeId
        description: The list of issue type ids to further restrict the search
      - in: query
        name: maxResults
        description: the maximum number of users to return (defaults to 50)
      - in: query
        name: projectId
        description: The list of project ids to further restrict the search This parameter
          can occur multiple times to pass in multiple project ids
      - in: query
        name: query
        description: A string used to search username, Name or e-mail address
      - in: query
        name: showAvatar
        description: If the user avatar should be returned or not
      responses:
        200:
          description: OK
      tags:
      - Find
      - Users
      - Groups
  /api/2/user/assignable/multiProjectSearch:
    get:
      summary: Find users assignable to projects
      description: |-
        Returns a list of users who fulfill both of these criteria:

        *   their user attributes match a string.
        *   they can be assigned issues in one or more projects.

        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** None.
      operationId: com.atlassian.jira.rest.v2.issue.UserResource.findBulkAssignableUsers_get
      x-api-path-slug: api2userassignablemultiprojectsearch-get
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: projectKeys
        description: A comma-separated list of project keys (case sensitive)
      - in: query
        name: query
        description: A search input that is matched against appropriate user attributes
          to find relevant users
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      - in: query
        name: username
        description: The search string
      responses:
        200:
          description: OK
      tags:
      - Find
      - Users
      - Assignable
      - To
      - Projects
  /api/2/user/assignable/search:
    get:
      summary: Find users assignable to issues
      description: |-
        Returns a list of users that can be assigned to an issue. Use this method to find the list of users who can be assigned to:

        *   a new issue, by providing the `projectKeyOrId`.
        *   an updated issue, by providing the `issueKey`.
        *   to an issue during a transition (workflow action), by providing the `issueKey` and the transition id in `actionDescriptorId`. You can obtain the IDs of an issue's valid transitions using the `transitions` option in the `expand` parameter of [Get issue](https://developer.atlassian.com/cloud/jira/platform/rest/#api-api-2-issue-issueIdOrKey-get).

        In all these cases, you can pass a username to determine if a user can be assigned to an issue. The user is returned in the response if they can be assigned to the issue or issue transition. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission to access Jira.
      operationId: com.atlassian.jira.rest.v2.issue.UserResource.findAssignableUsers_get
      x-api-path-slug: api2userassignablesearch-get
      parameters:
      - in: query
        name: actionDescriptorId
        description: The ID of the transition
      - in: header
        name: force-account-id
      - in: query
        name: issueKey
        description: The key of the issue
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: project
        description: The project ID or project key (case sensitive)
      - in: query
        name: query
        description: A search input that is matched against appropriate user attributes
          to find relevant users
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      - in: query
        name: username
        description: The username of the user
      responses:
        200:
          description: OK
      tags:
      - Find
      - Users
      - Assignable
      - To
      - Issues
  /api/2/user/permission/search:
    get:
      summary: Find users with permissions
      description: |-
        Returns a list of users who fulfill both of these criteria:

        *   their user attributes match a search string.
        *   they have a set of permissions for a project or issue.

        If no search string is provided, a list of all users with the permissions is returned. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   Get users for any project, _Administer Jira_ [global permission](href=).
        *   Get users for a project, _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg) for the project.
      operationId: com.atlassian.jira.rest.v2.issue.UserResource.findUsersWithAllPermissions_get
      x-api-path-slug: api2userpermissionsearch-get
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: issueKey
        description: The issue key for the issue
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: permissions
        description: A comma-separated list of permissions
      - in: query
        name: projectKey
        description: The project key for the project (case sensitive)
      - in: query
        name: query
        description: A search input that is matched against appropriate user attributes
          to find relevant users
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      - in: query
        name: username
        description: The search string
      responses:
        200:
          description: OK
      tags:
      - Find
      - Users
      - Permissions
  /api/2/user/picker:
    get:
      summary: Find users for picker
      description: Returns a list of users whose attributes match the query term.
        The returned object includes the `html` field where the matched query term
        is highlighted with the HTML strong tag. A list of usernames can be provided
        to exclude users from the results. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** _Browse users and groups_ [global permission](href=). Users with
        permission to access Jira can call this method, but will only get search results
        for an exact name match.
      operationId: com.atlassian.jira.rest.v2.issue.UserResource.findUsersForPicker_get
      x-api-path-slug: api2userpicker-get
      parameters:
      - in: query
        name: exclude
        description: A comma-separated list of usernames to exclude from the search
          results
      - in: query
        name: excludeAccountIds
        description: A comma-separated list of user accountIds to exclude from the
          search results
      - in: header
        name: force-account-id
      - in: query
        name: maxResults
        description: The maximum number of items to return
      - in: query
        name: query
        description: A search input that is matched against appropriate user attributes
          to find relevant users
      - in: query
        name: showAvatar
        description: Include the URI to the users avatar
      responses:
        200:
          description: OK
      tags:
      - Find
      - Userspicker
  /api/2/user/search:
    get:
      summary: Find users
      description: Returns a list of users that match the search string and property.
        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse
        users and groups_ [global permission](href=). Users with permission to access
        Jira can call this method, but empty search results are returned.
      operationId: com.atlassian.jira.rest.v2.issue.UserResource.findUsers_get
      x-api-path-slug: api2usersearch-get
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: includeActive
        description: Include active users
      - in: query
        name: includeInactive
        description: Include inactive users
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: property
        description: A query string used to search properties
      - in: query
        name: query
        description: A search input that is matched against appropriate user attributes
          to find relevant users
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      - in: query
        name: username
        description: A query string used to search username, display name, and email
          address
      responses:
        200:
          description: OK
      tags:
      - Find
      - Users
  /api/2/user/search/query:
    get:
      summary: Find users by query
      description: |-
        Finds users using a structured query and returns user details. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse users and groups_ [global permission](href=). The available queries statements are:

        `is assignee of PROJ` Returns the users that are assignees of at least one issue in project _PROJ_.*   `is assignee of (PROJ-1, PROJ-2)` Returns users that are assignees on the issues _PROJ-1_ or _PROJ-2_.
        *   `is reporter of (PROJ-1, PROJ-2)` Returns users that are reporters on the issues _PROJ-1_ or _PROJ-2_.
        *   `is watcher of (PROJ-1, PROJ-2)` Returns users that are watchers on the issues _PROJ-1_ or _PROJ-2_.
        *   `is voter of (PROJ-1, PROJ-2)` Returns users that are voters on the issues _PROJ-1_ or _PROJ-2_.
        *   `is commenter of (PROJ-1, PROJ-2)` Returns users that have posted a comment on the issues _PROJ-1_ or _PROJ-2_.
        *   `is transitioner of (PROJ-1, PROJ-2)` Returns users that have performed a transition on issues _PROJ-1_ or _PROJ-2_.
        *   `[propertyKey].entity.property.path is "property value"` Returns users with the entity property value.

        The list of issues can be extended as needed, as in _(PROJ-1, PROJ-2, ... PROJ-n)_. Statements can be combined using the `AND` and `OR` operators to form more complex queries, for example:

        `is assignee of PROJ AND [propertyKey].entity.property.path is "property value"`
      operationId: com.atlassian.jira.rest.v2.search.UserSearchResource.findUsersByQuery_get
      x-api-path-slug: api2usersearchquery-get
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: includeInactive
        description: Include inactive users in the results
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: query
        description: The search query
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      responses:
        200:
          description: OK
      tags:
      - Find
      - Users
      - By
      - Query
  /api/2/user/search/query/key:
    get:
      summary: Find user keys by query
      description: |-
        Finds users using a structured query and returns a list of user keys. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** _Browse users and groups_ [global permission](href=). The available query statements are:

        *   `is assignee of PROJ` Returns the users that are assignees of at least one issue in project _PROJ_.
        *   `is assignee of (PROJ-1, PROJ-2)` Returns users that are assignees on the issues _PROJ-1_ or _PROJ-2_.
        *   `is reporter of (PROJ-1, PROJ-2)` Returns users that are reporters on the issues _PROJ-1_ or _PROJ-2_.
        *   `is watcher of (PROJ-1, PROJ-2)` Returns users that are watchers on the issues _PROJ-1_ or _PROJ-2_.
        *   `is voter of (PROJ-1, PROJ-2)` Returns users that are voters on the issues _PROJ-1_ or _PROJ-2_.
        *   `is commenter of (PROJ-1, PROJ-2)` Returns users that have posted a comment on the issues _PROJ-1_ or _PROJ-2_.
        *   `is transitioner of (PROJ-1, PROJ-2)` Returns users that have performed a transition on issues _PROJ-1_ or _PROJ-2_.
        *   `[propertyKey].entity.property.path is "property value"` Returns users with the entity property value.

        The list of issues can be extended as needed, as in _(PROJ-1, PROJ-2, ... PROJ-n)_. Statements can be combined using the `AND` and `OR` operators to form more complex queries, for example:

        `is assignee of PROJ AND [propertyKey].entity.property.path is "property value"`
      operationId: com.atlassian.jira.rest.v2.search.UserSearchResource.findUserKeysByQuery_get
      x-api-path-slug: api2usersearchquerykey-get
      parameters:
      - in: header
        name: force-account-id
      - in: query
        name: includeInactive
        description: Include inactive users in the results
      - in: query
        name: maxResults
        description: The maximum number of items to return per page
      - in: query
        name: query
        description: The search query
      - in: query
        name: startAt
        description: The index of the first item to return in a page of results (page
          offset)
      responses:
        200:
          description: OK
      tags:
      - Find
      - User
      - Keys
      - By
      - Query
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