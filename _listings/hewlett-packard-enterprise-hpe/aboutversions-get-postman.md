{
  "info": {
    "name": "HPE OneSphere API Get About Versions",
    "_postman_id": "9301fa7e-4f9b-4895-8644-9e3824612541",
    "description": "Get supported versions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "About",
      "item": [
        {
          "id": "ded984c8-4f95-4089-a59d-d25580c2c07c",
          "name": "GetVersions",
          "request": {
            "url": "http://deic02-hpe.hpeonesphere.com/rest/about/versions",
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
            "description": "Get supported versions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9784b95-6314-43d6-9269-bc001e4d359b"
            }
          ]
        }
      ]
    }
  ]
}