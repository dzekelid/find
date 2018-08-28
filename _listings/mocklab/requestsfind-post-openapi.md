---
swagger: "2.0"
x-collection-name: MockLab
x-complete: 0
info:
  title: MockLab Post Requests Find
  version: 1.0.0
  description: Retrieve details of requests logged in the journal matching the specified
    criteria
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