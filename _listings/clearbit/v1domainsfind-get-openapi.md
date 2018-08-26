---
swagger: "2.0"
x-collection-name: Clearbit
x-complete: 0
info:
  title: Clearbit Company Name to Domain
  description: 'TODO: Add Description'
  version: 1.0.0
host: discovery.clearbit.com
basePath: /v1/companies
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/companies/find:
    get:
      summary: Domain Lookup
      description: 'TODO: Add Description'
      operationId: V2CompaniesFindGet
      x-api-path-slug: v2companiesfind-get
      parameters:
      - in: query
        name: domain
      responses:
        200:
          description: OK
      tags:
      - Companies
      - Find
  /find:
    get:
      summary: Find Company by IP Address
      description: 'TODO: Add Description'
      operationId: FindGet2
      x-api-path-slug: find-get
      parameters:
      - in: query
        name: ip
      responses:
        200:
          description: OK
      tags:
      - Find
  /v1/domains/find:
    get:
      summary: Company Name to Domain
      description: 'TODO: Add Description'
      operationId: V1DomainsFindGet
      x-api-path-slug: v1domainsfind-get
      parameters:
      - in: query
        name: name
      responses:
        200:
          description: OK
      tags:
      - Domains
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