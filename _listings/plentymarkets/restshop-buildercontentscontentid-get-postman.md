{
  "info": {
    "name": "Plentymarkets Find a content by id.",
    "_postman_id": "ba2af9d9-dcff-4a1f-9ce4-0a5ab9186476",
    "description": "Find a content by id..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Find",
      "item": [
        {
          "id": "25311fb5-94df-4b46-a98f-19879188eb34",
          "name": "getRestAccountsAddressesAddressRelatedData",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/addresses/:addressId/related_data"
              ],
              "variable": [
                {
                  "id": "addressId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Find address data by address id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17c7aa4c-afce-4886-9a7a-0aba2204dbc9"
            }
          ]
        },
        {
          "id": "4c2b9046-3bb5-41d8-856d-5f5abf659006",
          "name": "getRestBackendUsersSearchNameName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/backend/users/search_name/:name"
              ],
              "variable": [
                {
                  "id": "name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Find all users having a name or username like the given one.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6fa0f3f-c3c0-4bdd-89d8-8818454012cc"
            }
          ]
        },
        {
          "id": "a61bfa82-59f1-4a9a-a869-67f9f0c50eaf",
          "name": "getRestBasketItems",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/basket/items/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Find a basket item by it's id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c546fa09-e6fd-44d4-8e6c-3942de86bb4f"
            }
          ]
        },
        {
          "id": "d205f8eb-7c72-46ac-8639-8a2b23541dbf",
          "name": "getRestListingsMarketsFind",
          "request": {
            "url": "http://example.com/rest/listings/markets/find?credentialsId=%7B%7D&directoryId=%7B%7D&id=%7B%7D&itemId=%7B%7D&itemsPerPage=%7B%7D&page=%7B%7D&referrerId=%7B%7D&shippingProfileId=%7B%7D&variations=%7B%7D&with=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists listing market by filter options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0f2e9ac-e398-4a6b-8863-63e0ca2bba2d"
            }
          ]
        },
        {
          "id": "56bcbd13-8b1b-47f6-ace1-ff80f332f5e9",
          "name": "getRestOrdersDatesTypesType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/orders/dates/types/:typeId"
              ],
              "variable": [
                {
                  "id": "typeId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Find an order date type by it's id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4333b0f8-9fe2-4032-9a7b-47a31eece904"
            }
          ]
        },
        {
          "id": "6af57fce-2403-4d49-a190-76378f75c65a",
          "name": "getRestShopBuilderContentLinksContentlink",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/shop_builder/content_links/:contentLinkId"
              ],
              "variable": [
                {
                  "id": "contentLinkId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Find a content link by id.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3abb8780-6dca-45bd-908e-ead268142565"
            }
          ]
        },
        {
          "id": "d55ed4f5-e934-4311-b354-281e6e4a8a8b",
          "name": "getRestShopBuilderContentsContent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/shop_builder/contents/:contentId"
              ],
              "variable": [
                {
                  "id": "contentId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Find a content by id.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a16d4ed-b1ca-40cb-aaa8-ab84467bb72a"
            }
          ]
        }
      ]
    }
  ]
}