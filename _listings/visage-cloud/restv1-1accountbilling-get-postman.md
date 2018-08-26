{
  "info": {
    "name": "Visage Cloud Get billing information by accessKey and secretKey",
    "_postman_id": "f5c5538a-bf71-4e1f-a8ff-89c69c33b614",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "36fd5be8-5f9f-4657-94e3-7d8b82c774f2",
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
          "id": "c8f395f6-d941-458c-b6e0-5864e07722f3"
        }
      ]
    },
    {
      "id": "dcff63ff-cd8f-421e-a32f-bab3c7d44258",
      "name": "getBillingPerAccountUsingGET",
      "request": {
        "url": "http://visagecloud.com/rest/v1.1/account/billing?accessKey=%7B%7D&dateTemplate=%7B%7D&endDateTime=%7B%7D&secretKey=%7B%7D&startDateTime=%7B%7D",
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
        "description": "Get billing information by accessKey and secretKey"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "442d1cd4-1996-4c72-ba2f-5b4423f86d9e"
        }
      ]
    }
  ]
}