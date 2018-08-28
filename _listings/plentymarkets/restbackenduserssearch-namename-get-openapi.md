---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Find all users having a name or username like the given one.
  description: Find all users having a name or username like the given one..
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/addresses/{addressId}/related_data:
    get:
      summary: Find address data by address id
      description: Find address data by address id.
      operationId: getRestAccountsAddressesAddressRelatedData
      x-api-path-slug: restaccountsaddressesaddressidrelated-data-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Address
      - Data
      - By
      - Address
      - Id
  /rest/backend/users/search_name/{name}:
    get:
      summary: Find all users having a name or username like the given one.
      description: Find all users having a name or username like the given one..
      operationId: getRestBackendUsersSearchNameName
      x-api-path-slug: restbackenduserssearch-namename-get
      parameters:
      - in: path
        name: name
      responses:
        200:
          description: OK
      tags:
      - Find
      - ""
      - Users
      - Having
      - Name
      - Username
      - Like
      - Given
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