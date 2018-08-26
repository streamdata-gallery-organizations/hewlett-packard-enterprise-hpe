{
  "info": {
    "name": "HPE OneSphere API Get Catalog Types",
    "_postman_id": "569b1c1e-5e42-4365-8af2-5ce367c25a47",
    "description": "Returns catalog types.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Catalog",
      "item": [
        {
          "id": "16cfb8c7-37c7-46fe-ba0f-582a88621358",
          "name": "FindCatalogTypes",
          "request": {
            "url": "http://deic02-hpe.hpeonesphere.com/rest/catalog-types",
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
            "description": "Returns catalog types."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7feef295-a407-4ace-976f-f344435ab885"
            }
          ]
        }
      ]
    }
  ]
}