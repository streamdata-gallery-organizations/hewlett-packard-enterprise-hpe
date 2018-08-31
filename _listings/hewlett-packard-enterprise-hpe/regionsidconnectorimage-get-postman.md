{
  "info": {
    "name": "HPE OneSphere API Get Regions Connector Image",
    "_postman_id": "be9c53a2-e096-4733-b158-67cc0837011a",
    "description": "Generates connector-image url for the region. It requires the **administrator** role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Regions",
      "item": [
        {
          "id": "277df6c3-bf3b-47d2-9015-b256cd65b104",
          "name": "getConnectorImage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "deic02-hpe.hpeonesphere.com",
              "path": [
                "rest",
                "regions/:id/connector-image"
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
            "description": "Generates connector-image url for the region. It requires the **administrator** role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc480918-91f6-4266-8ad1-0d0136b813bc"
            }
          ]
        }
      ]
    }
  ]
}