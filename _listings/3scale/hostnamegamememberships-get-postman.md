{
  "info": {
    "name": "3scale Find Game Memberships",
    "_postman_id": "0e1d5df2-b648-4148-864d-50284ca60275",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "6dd700f6-212d-4d99-a8dc-6cdc4b794f67",
      "name": "GameMembershipsByHostnameGet",
      "request": {
        "url": {
          "protocol": "http",
          "host": "http",
          "path": [
            ":hostname/game-memberships"
          ],
          "query": [
            {
              "key": "filter[game_id]",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "hostname",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "x-client-auth",
            "value": "{}",
            "description": "",
            "disabled": false
          },
          {
            "key": "x-client-bearer-token",
            "value": "{}",
            "description": "",
            "disabled": false
          },
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Find Game Memberships"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "5c04ea17-d7d7-4281-87e7-666452287f37"
        }
      ]
    }
  ]
}