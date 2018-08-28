swagger: "2.0"
x-collection-name: Flickr
x-complete: 1
info:
  title: Flickr
  description: explore-upload-and-organize-photos-on-flickr
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