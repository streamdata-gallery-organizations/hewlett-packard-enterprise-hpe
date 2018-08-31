{
  "info": {
    "name": "HPE OneSphere API Get Billing Accounts",
    "_postman_id": "f177b38a-6a46-4611-84b2-a93181111689",
    "description": "Returns billing accounts. It requires the **administrator** or **project creator** global role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Billing",
      "item": [
        {
          "id": "84bc5fd4-dffc-498b-ab71-0cf9e847c253",
          "name": "FindBillingAccounts",
          "request": {
            "url": "http://deic02-hpe.hpeonesphere.com/rest/billing-accounts?query=%7B%7D&view=%7B%7D",
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
            "description": "Returns billing accounts. It requires the **administrator** or **project creator** global role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8dc3076-7426-4b68-b6f9-dda3a5ac324a"
            }
          ]
        }
      ]
    }
  ]
}