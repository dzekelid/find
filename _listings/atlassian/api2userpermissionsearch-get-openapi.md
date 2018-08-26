---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Find users with permissions
  description: |-
    Returns a list of users who fulfill both of these criteria:

    *   their user attributes match a search string.
    *   they have a set of permissions for a project or issue.

    If no search string is provided, a list of all users with the permissions is returned. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

    *   Get users for any project, _Administer Jira_ [global permission](href=).
    *   Get users for a project, _Administer Projects_ [project permission](https://confluence.atlassian.com/x/yodKLg) for the project.
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