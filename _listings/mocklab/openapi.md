swagger: "2.0"
x-collection-name: MockLab
x-complete: 1
info:
  title: WireMock
  version: 1.0.0
basePath: /__admin
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mappings/find-by-metadata:
    post:
      summary: Post Mappings Find By Metadata
      description: Find stubs by matching on their metadata
      operationId: postMappingsFindByMetadata
      x-api-path-slug: mappingsfindbymetadata-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Find
      - Metadata
  /requests/find:
    post:
      summary: Post Requests Find
      description: Retrieve details of requests logged in the journal matching the
        specified criteria
      operationId: postRequestsFind
      x-api-path-slug: requestsfind-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Requests
      - Find