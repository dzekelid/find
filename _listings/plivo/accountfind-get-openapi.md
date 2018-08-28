---
swagger: "2.0"
x-collection-name: Plivo
x-complete: 0
info:
  title: Codenvy Account API Get Account Find
  description: Get account information by its name. JSON with account details is returned.
    This API call requires system/admin or system/manager role.
  version: 1.0.0
host: /account
basePath: https://codenvy.com/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/find:
    get:
      summary: Get Account Find
      description: Get account information by its name. JSON with account details
        is returned. This API call requires system/admin or system/manager role.
      operationId: getByName
      x-api-path-slug: accountfind-get
      parameters:
      - in: query
        name: name
        description: Account name
      responses:
        200:
          description: OK
      tags:
      - Account
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