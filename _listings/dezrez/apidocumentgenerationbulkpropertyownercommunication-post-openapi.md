---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: "Dezrez Generates a bulk communication pack out to multiple vendors of properties.\r\nThis
    will ignore the target type set, as the document could only ever find the vendor
    as the contact item, so it always defaults\r\nto a target type of vendor/owner"
  version: 1.0.0
  description: "Generates a bulk communication pack out to multiple vendors of properties.\r\nthis
    will ignore the target type set, as the document could only ever find the vendor
    as the contact item, so it always defaults\r\nto a target type of vendor/owner."
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/bulkpropertyownercommunication:
    post:
      summary: "Generates a bulk communication pack out to multiple vendors of properties.\r\nThis
        will ignore the target type set, as the document could only ever find the
        vendor as the contact item, so it always defaults\r\nto a target type of vendor/owner"
      description: "Generates a bulk communication pack out to multiple vendors of
        properties.\r\nthis will ignore the target type set, as the document could
        only ever find the vendor as the contact item, so it always defaults\r\nto
        a target type of vendor/owner."
      operationId: DocumentGeneration_BulkPropertyVendorCommunicationBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationbulkpropertyownercommunication-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Bulk
      - Communication
      - Pack
      - Out
      - To
      - Multiple
      - Vendors
      - Of
      - Properties
      - This
      - Will
      - Ignore
      - Target
      - Type
      - Set
      - ""
      - As
      - Document
      - Could
      - Only
      - Ever
      - Find
      - Vendor
      - As
      - Contact
      - Item
      - ""
      - So
      - It
      - Always
      - "Defaults\r\nTo"
      - Target
      - Type
      - Of
      - Vendor
      - Owner
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