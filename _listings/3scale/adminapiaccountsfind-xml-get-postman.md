{
  "info": {
    "name": "3Scale Account Management API Account Find",
    "_postman_id": "bf738362-2a0a-44b5-86c2-141315b5f761",
    "description": "Account find.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "95323c90-9e0c-4957-8766-663a28c12843",
          "name": "account",
          "request": {
            "url": "http://su1.3scale.net/admin/api/accounts.xml?page=%7B%7D&per_page=%7B%7D&provider_key=%7B%7D&state=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e16fb7b-fce7-44ed-83b9-ddf8204f7e06"
            }
          ]
        },
        {
          "id": "4a676114-0866-40a2-b7c6-e8acaeca4e8e",
          "name": "account",
          "request": {
            "url": "http://su1.3scale.net/admin/api/accounts/find.xml?email=%7B%7D&provider_key=%7B%7D&username=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account find."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27f5ae7c-a7ac-4040-98ca-600887c36b6d"
            }
          ]
        }
      ]
    }
  ]
}