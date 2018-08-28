---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Find groups
  description: |-
    Returns groups with substrings matching a given query. This is mainly for use with the group picker, so the returned groups contain html to be used as picker suggestions. The groups are also wrapped in a single response object that also contains a header for use in the picker, specifically _Showing X of Y matching groups_.

    The number of groups returned is limited by the system property "jira.ajax.autocomplete.limit"

    The groups will be unique and sorted.
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