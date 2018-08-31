{
  "info": {
    "name": "HPE OneSphere API Get Events",
    "_postman_id": "45448b50-749e-4976-a228-08594e88d4f9",
    "description": "Returns events based on the supplied criteria. **Not implemented**",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "40d331fa-e064-4475-9a32-810ce48aa55a",
          "name": "FindEvents",
          "request": {
            "url": "http://deic02-hpe.hpeonesphere.com/rest/events?resourceUri=%7B%7D",
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
            "description": "Returns events based on the supplied criteria. **Not implemented**"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9068712-cd24-48ad-bfa8-fc2dfbfe3174"
            }
          ]
        }
      ]
    }
  ]
}