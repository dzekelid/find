---
swagger: "2.0"
x-collection-name: 3scale
x-complete: 0
info:
  title: 3scale Find Games
  description: ""
  version: "1.0"
host: 'http:'
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  //{hostname}/game-memberships:
    get:
      summary: Find Game Memberships
      description: ""
      operationId: GameMembershipsByHostnameGet
      x-api-path-slug: hostnamegamememberships-get
      parameters:
      - in: query
        name: filter[game_id]
      - in: path
        name: hostname
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/game-rounds:
    get:
      summary: Find Game Rounds
      description: ""
      operationId: GameRoundsByHostnameGet
      x-api-path-slug: hostnamegamerounds-get
      parameters:
      - in: query
        name: filter[game_id]
      - in: path
        name: hostname
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
  //{hostname}/games:
    get:
      summary: Find Games
      description: ""
      operationId: GamesByHostnameGet
      x-api-path-slug: hostnamegames-get
      parameters:
      - in: path
        name: hostname
      - in: header
        name: x-client-auth
      - in: header
        name: x-client-bearer-token
      responses:
        200:
          description: OK
      tags:
      - ""
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