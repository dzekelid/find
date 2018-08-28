swagger: "2.0"
x-collection-name: 3scale
x-complete: 1
info:
  title: 3scale Service Management API
  description: the-api-for-managing-3scale-services-
  termsOfService: http://www.3scale.net/terms-and-conditions/
  contact:
    name: 3Scale
    url: https://support.3scale.net/
  version: "1"
host: su1.3scale.net
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
  /admin/api/accounts/find.xml:
    get:
      summary: Account Find
      description: Account find.
      operationId: account
      x-api-path-slug: adminapiaccountsfind-xml-get
      parameters:
      - in: query
        name: email
        description: email of the user of the account
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: username
        description: username of the user of the account
      - in: query
        name: user_id
        description: id of the user of the account
      responses:
        200:
          description: OK
      tags:
      - Account
      - Find
  /admin/api/applications/find.xml:
    get:
      summary: Application Find
      description: Application find.
      operationId: application
      x-api-path-slug: adminapiapplicationsfind-xml-get
      parameters:
      - in: query
        name: application_id
        description: id of the application
      - in: query
        name: app_id
        description: app_id of the application (for app_id/app_key and oauth authentication
          modes)
      - in: query
        name: provider_key
        description: Your api key with 3scale (also known as provider key)
      - in: query
        name: user_key
        description: user_key of the application (for user_key authentication mode)
      responses:
        200:
          description: OK
      tags:
      - Application
      - Find