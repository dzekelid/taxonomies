{
  "info": {
    "name": "reverb Get Categories Taxonomy",
    "_postman_id": "7853ea27-f008-434e-a8d5-5cb7218e3b8b",
    "description": "Full taxonomy tree of categories including middle categories",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "50ac4270-b530-41ef-8894-965deda238dc",
          "name": "getCategories",
          "request": {
            "url": "http://api.reverb.com/api/categories",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of supported product categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0ddfba4-3905-4e96-a302-9ad47f4c5f15"
            }
          ]
        },
        {
          "id": "97f2f1ef-efd2-49b6-a527-ad55bcac4c58",
          "name": "getCategoriesFlat",
          "request": {
            "url": "http://api.reverb.com/api/categories/flat",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get categories flat."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9de5b147-2305-4efc-b826-b7d8ed8b13cf"
            }
          ]
        },
        {
          "id": "f17ad038-1439-4b93-8f96-a37762f56840",
          "name": "getCategoriesTaxonomy",
          "request": {
            "url": "http://api.reverb.com/api/categories/taxonomy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Full taxonomy tree of categories including middle categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa6c5308-d9c8-4ca9-9f4a-eb082409f8ed"
            }
          ]
        }
      ]
    }
  ]
}