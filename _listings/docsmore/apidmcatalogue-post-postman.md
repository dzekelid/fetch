{
  "info": {
    "name": "Docsmore Fetch All Documents from Your Team Catalogue",
    "_postman_id": "de04dbfb-3263-4421-ba68-066f418f4799",
    "description": "By design, the authenticated user can only view the files that are either created by them or shared with them. Make sure user has at least read permission to view the catalogue.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Fetch",
      "item": [
        {
          "id": "a329f99b-c010-43de-9b7f-d6ed1ab397d1",
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
              "id": "5ed564ab-be6c-4984-a59b-29d673b26db5"
            }
          ]
        }
      ]
    }
  ]
}