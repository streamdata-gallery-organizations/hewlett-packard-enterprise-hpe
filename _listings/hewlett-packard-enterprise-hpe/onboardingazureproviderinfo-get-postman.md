{
  "info": {
    "name": "HPE OneSphere API Get Onboarding Azure Prover Info",
    "_postman_id": "973e1268-79f6-477d-a3b8-67a78b520bd6",
    "description": "Returns the provider information required to add an Azure provider",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Onboarding",
      "item": [
        {
          "id": "c8024143-257f-4539-9c8d-865a3d1801fe",
          "name": "getAzureProviderInfo",
          "request": {
            "url": "http://deic02-hpe.hpeonesphere.com/rest/onboarding/azure/provider-info?directoryUri=%7B%7D&location=%7B%7D",
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
            "description": "Returns the provider information required to add an Azure provider"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21b3e55c-42fa-4167-8077-7aaceeed6013"
            }
          ]
        }
      ]
    }
  ]
}