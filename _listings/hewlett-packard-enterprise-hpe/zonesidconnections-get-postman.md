{
  "info": {
    "name": "HPE OneSphere API Get Zones Connections",
    "_postman_id": "03d92848-de3b-4a3d-8aaf-9a79d48600ad",
    "description": "Gets the list of connection for the zone. It requires the **administrator** role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Zones",
      "item": [
        {
          "id": "bafd4a60-8e68-47cc-8197-be869380a025",
          "name": "zoneConnectionInstances",
          "request": {
            "url": {
              "protocol": "http",
              "host": "deic02-hpe.hpeonesphere.com",
              "path": [
                "rest",
                "zones/:id/connections"
              ],
              "query": [
                {
                  "key": "uuid",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Gets the list of connection for the zone. It requires the **administrator** role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e31aedc3-cb9a-455b-8760-e928c9295bb7"
            }
          ]
        }
      ]
    }
  ]
}