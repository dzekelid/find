{
  "info": {
    "name": "Plentymarkets Find listing markets",
    "_postman_id": "bbbf7e9b-bc9d-493e-a9a6-047cc8c96cbf",
    "description": "Lists listing market by filter options.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Find",
      "item": [
        {
          "id": "76da1623-6302-4fcc-a987-11a02c017f53",
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
              "id": "1e0174c7-f35a-4f5c-a6e0-d474f80fda29"
            }
          ]
        },
        {
          "id": "4aff6214-1232-4564-af37-9e7bbfecebd5",
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
              "id": "55890230-686a-44e5-8439-536a78e6678b"
            }
          ]
        },
        {
          "id": "59fb11a4-ff94-499a-b0cb-926caaf93de9",
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
              "id": "04301d59-4fb3-4a8e-b334-cfc7940933c0"
            }
          ]
        },
        {
          "id": "842d9ac1-ef22-4960-a9cb-cff5a81a1bb8",
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
              "id": "7775df77-138d-43ae-8ad1-a0b5376f8c41"
            }
          ]
        }
      ]
    }
  ]
}