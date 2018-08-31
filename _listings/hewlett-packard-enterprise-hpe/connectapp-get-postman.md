{
  "info": {
    "name": "HPE OneSphere API Get Connect App",
    "_postman_id": "fe6f2a39-247b-42a4-88a1-5648c8cc0b74",
    "description": "Generates connect app s3 url",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Connect",
      "item": [
        {
          "id": "bcc3e5bf-af83-4883-8ab9-b01e8730e96c",
          "name": "connect-app",
          "request": {
            "url": "http://deic02-hpe.hpeonesphere.com/rest/connect-app?os=%7B%7D",
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
            "description": "Generates connect app s3 url"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24cd760a-ade9-4304-86f7-c5716a498022"
            }
          ]
        }
      ]
    }
  ]
}