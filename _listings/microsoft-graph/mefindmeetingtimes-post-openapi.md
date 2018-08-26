---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph User Find Meeting Times
  description: 'user: findMeetingTimes Find meeting time suggestions based on organizer
    and attendee availability, and time or location constraints specified as parameters.'
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