{
  "info": {
    "name": "Plentymarkets Find an order date type by it's ID",
    "_postman_id": "4a8eb8ea-08a8-4063-826a-5f93d5a28d5b",
    "description": "Find an order date type by it's id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Find",
      "item": [
        {
          "id": "3378759c-c7bb-44ca-8ec4-870f3868db4a",
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
              "id": "b99a2e2a-d7f7-4516-9f49-30f50eeb8070"
            }
          ]
        },
        {
          "id": "8bd9462c-c8a1-4640-bbf0-3ce795116948",
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
              "id": "65ed782e-5811-447e-803e-150d72d3952f"
            }
          ]
        },
        {
          "id": "2c2f77ac-15bc-45a0-b7ce-322926de7699",
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
              "id": "cf440671-caf6-47f0-8df0-4e2a276db5db"
            }
          ]
        },
        {
          "id": "d80bd92d-27ec-45fb-a5d8-5bf587c453b3",
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
              "id": "f0eca1ce-c010-4bd7-97e7-ab80052f0016"
            }
          ]
        },
        {
          "id": "e7a158e5-1b3b-47a4-b12c-4527e90a9195",
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
              "id": "f864dadc-16d1-4086-b7c6-bdc276f09f38"
            }
          ]
        }
      ]
    }
  ]
}