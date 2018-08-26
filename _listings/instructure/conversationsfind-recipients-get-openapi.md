---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Conversations API Find recipients
  description: Find recipients.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /conversations/find_recipients:
    get:
      summary: Find recipients
      description: Find recipients.
      operationId: find-recipients
      x-api-path-slug: conversationsfind-recipients-get
      parameters:
      - in: query
        name: context
        description: Limit the search to a particular course/group (e
      - in: query
        name: exclude[]
        description: Array of ids to exclude from the search
      - in: query
        name: from_conversation_id
        description: When searching by user_id, only users that could be normally
          messaged bynthis user will be returned
      - in: query
        name: permissions[]
        description: Array of permission strings to be checked for each matched context
          (e
      - in: query
        name: search
        description: Search terms used for matching users/courses/groups (e
      - in: query
        name: type
        description: Limit the search just to users or contexts (groups/courses)
      - in: query
        name: user_id
        description: Search for a specific user id
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Find
      - Recipients
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