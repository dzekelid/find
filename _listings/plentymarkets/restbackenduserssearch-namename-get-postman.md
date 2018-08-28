{
  "info": {
    "name": "Plentymarkets Find all users having a name or username like the given one.",
    "_postman_id": "c6949017-e6f5-4659-ab9b-b6e7326b656d",
    "description": "Find all users having a name or username like the given one..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Find",
      "item": [
        {
          "id": "d96a65a4-00bc-420d-a847-e974ce006d47",
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
              "id": "c894d24b-b4c9-48f6-9c21-aded2940ce21"
            }
          ]
        },
        {
          "id": "65875f5e-9000-43da-a039-719648585379",
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
              "id": "de2d289e-6d5d-48b0-af44-e7abe397b1da"
            }
          ]
        }
      ]
    }
  ]
}