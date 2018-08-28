swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/findMeetingTimes:
    post:
      summary: User Find Meeting Times
      description: 'user: findMeetingTimes Find meeting time suggestions based on
        organizer and attendee availability, and time or location constraints specified
        as parameters.'
      operationId: User:FindMeetingTimes
      x-api-path-slug: mefindmeetingtimes-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: 'Prefer: outlook.timezone'
        description: A string representing a specific time zone for the response,
          for example, Pacific Standard Time
      responses:
        200:
          description: OK
      tags:
      - User
      - Find
      - Meeting
      - Times
  /users/{id|userPrincipalName}/findMeetingTimes:
    post:
      summary: User Find Meeting Times
      description: 'user: findMeetingTimes Find meeting time suggestions based on
        organizer and attendee availability, and time or location constraints specified
        as parameters.'
      operationId: User:FindMeetingTimes
      x-api-path-slug: usersiduserprincipalnamefindmeetingtimes-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id|userPrincipalName
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: A string representing a specific time zone for the response,
          for example, Pacific Standard Time
      responses:
        200:
          description: OK
      tags:
      - User
      - Find
      - Meeting
      - Times