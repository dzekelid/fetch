{
  "info": {
    "name": "Docsmore Fetch Single Document",
    "_postman_id": "de186a4e-4b53-4331-b9e7-304c9b4b0f51",
    "description": "Fetch single document.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Fetch",
      "item": [
        {
          "id": "68f2ef8d-2293-49e2-849c-13af5ff17e9e",
          "name": "ApiDmcataloguePost",
          "request": {
            "url": "http://api.docsmore.com/api/dmcatalogue?items=%7B%7D&page=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "By design, the authenticated user can only view the files that are either created by them or shared with them. Make sure user has at least read permission to view the catalogue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3321288-9715-4ebc-aa85-cd40e85307dd"
            }
          ]
        },
        {
          "id": "47bd699f-c157-44b6-b1c0-746b73a032ca",
          "name": "ApiDmcatalogueIdPost",
          "request": {
            "url": "http://api.docsmore.com/api/dmcatalogue/:id?id=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Fetch single document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2fabc9d-a687-4d20-bcf6-c0c276b422f3"
            }
          ]
        }
      ]
    }
  ]
}