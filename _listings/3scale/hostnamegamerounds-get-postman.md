{
  "info": {
    "name": "3scale Find Game Rounds",
    "_postman_id": "675adbe9-af43-4d5a-aa98-e926f7757b83",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "49e583e7-10e0-4d72-8c05-5291d897616b",
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
          "id": "fc7e644c-c012-4052-acda-6d702b05d282"
        }
      ]
    },
    {
      "id": "5f03a810-4218-4c41-b2c6-39859c3c030b",
      "name": "GameRoundsByHostnameGet",
      "request": {
        "url": {
          "protocol": "http",
          "host": "http",
          "path": [
            ":hostname/game-rounds"
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
        "description": "Find Game Rounds"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "89e877fa-2ba1-4612-b76b-c9a36bab0005"
        }
      ]
    }
  ]
}