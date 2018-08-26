---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Places Find
  description: Return a list of place IDs for a query string.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.places.find:
    get:
      summary: Places Find
      description: Return a list of place IDs for a query string.
      operationId: getRestMethodFlickr.places.find
      x-api-path-slug: restmethodflickr-places-find-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: query
        description: The query string to use for place ID lookups
      responses:
        200:
          description: OK
      tags:
      - Places
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