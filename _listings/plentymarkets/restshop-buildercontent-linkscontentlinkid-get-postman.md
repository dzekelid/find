{
  "info": {
    "name": "Plentymarkets Find a content link by id.",
    "_postman_id": "fcec8a56-c3e5-4a60-99bc-0d4d0fdb1a2b",
    "description": "Find a content link by id..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Find",
      "item": [
        {
          "id": "8f8e47ee-a883-4848-bed0-57c9dda5f151",
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
              "id": "0e23f5f9-9545-45e5-8bf6-b74c9b3c2b42"
            }
          ]
        },
        {
          "id": "25cd164a-a14c-441c-ae4e-6cf421b095a5",
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
              "id": "987a894a-322e-4815-b321-73d77878fa54"
            }
          ]
        },
        {
          "id": "bc170f85-12c0-4637-867c-fb69fe6121c2",
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
              "id": "d671dd38-4d95-41e5-8d47-19a1ce4f2558"
            }
          ]
        },
        {
          "id": "90ac0f76-7a56-43b8-ad83-aabed01539f9",
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
              "id": "42c4416a-b44e-4b56-8d7d-f83246f7fcc9"
            }
          ]
        },
        {
          "id": "22ca3068-8a63-40be-9b97-252eb62afbd0",
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
              "id": "e5955181-77f9-44f2-9f85-76f1861aea41"
            }
          ]
        },
        {
          "id": "6c4f142b-7e3b-46f8-9ac4-2c97ecbe4c5c",
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
              "id": "57323e44-0d0b-45f6-b021-3cd2f60d9862"
            }
          ]
        }
      ]
    }
  ]
}