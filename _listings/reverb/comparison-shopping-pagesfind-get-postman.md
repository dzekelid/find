{
  "info": {
    "name": "reverb Get Comparison Shopping Pages Find",
    "_postman_id": "81489509-5f8d-4ee9-8251-ed9d15b4684d",
    "description": "Get comparison shopping pages find.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Comparison",
      "item": [
        {
          "id": "6ffc8eef-00f0-4c54-9c9e-74f235b99980",
          "name": "getComparisonShoppingPages",
          "request": {
            "url": "http://api.reverb.com/api/comparison_shopping_pages",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a set of comparison shopping pages based on the current params"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2972337-ceae-45d8-99a2-f1acc3d38ef9"
            }
          ]
        },
        {
          "id": "6544ee9a-3d04-4505-9ff3-b5b7e635d1c7",
          "name": "getComparisonShoppingPagesFind",
          "request": {
            "url": "http://api.reverb.com/api/comparison_shopping_pages/find?id=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get comparison shopping pages find."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5307bef3-e6f9-4f7f-88bf-bfa0f4054cdb"
            }
          ]
        }
      ]
    }
  ]
}