---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Find a content link by id.
  description: Find a content link by id..
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
  /rest/basket/items/{id}:
    get:
      summary: Find a basket item by it's ID
      description: Find a basket item by it's id.
      operationId: getRestBasketItems
      x-api-path-slug: restbasketitemsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Find
      - Basket
      - Item
      - By
      - Its
      - ID
  /rest/listings/markets/find:
    get:
      summary: Find listing markets
      description: Lists listing market by filter options.
      operationId: getRestListingsMarketsFind
      x-api-path-slug: restlistingsmarketsfind-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing markets with
          given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing markets with
          a given directory ID
      - in: query
        name: id
        description: Filter that restricts the search result to listing markets that
          match the given ID(s)
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing markets that
          belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing markets with
          given referrer ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing markets that
          belong to a given shipping profile ID
      - in: query
        name: variations
        description: Filter that restricts the search result to listing markets with
          a custom variation condition
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Find
      - Listing
      - Markets
  /rest/orders/dates/types/{typeId}:
    get:
      summary: Find an order date type by it's ID
      description: Find an order date type by it's id.
      operationId: getRestOrdersDatesTypesType
      x-api-path-slug: restordersdatestypestypeid-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Order
      - Date
      - Type
      - By
      - Its
      - ID
  /rest/shop_builder/content_links/{contentLinkId}:
    get:
      summary: Find a content link by id.
      description: Find a content link by id..
      operationId: getRestShopBuilderContentLinksContentlink
      x-api-path-slug: restshop-buildercontent-linkscontentlinkid-get
      parameters:
      - in: path
        name: contentLinkId
      responses:
        200:
          description: OK
      tags:
      - Find
      - Content
      - Link
      - By
      - Id
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