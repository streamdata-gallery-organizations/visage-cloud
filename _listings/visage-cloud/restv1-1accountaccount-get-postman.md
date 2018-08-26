{
  "info": {
    "name": "Visage Cloud Get account information by accessKey and secretKey",
    "_postman_id": "25385819-a89c-4427-af92-21ef0ad517ee",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "3e298d7a-1586-4047-bbe3-f1e9f1b71726",
      "name": "getAccountByAccessKeyUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/account/account?accessKey=%7B%7D&secretKey=%7B%7D",
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
        "description": "Get account information by accessKey and secretKey"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "222b6ad5-fd8c-4204-a7aa-37b632664ee9"
        }
      ]
    }
  ]
}