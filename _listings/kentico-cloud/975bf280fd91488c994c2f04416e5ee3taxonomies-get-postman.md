{
  "info": {
    "name": "Kentico Cloud List taxonomy groups",
    "_postman_id": "c9a391b3-e2a0-4638-96e3-978f9b8c7752",
    "description": "Retrieve a paginated list of taxonomy groups in your project.\n\nBy default, the API returns all taxonomy groups ordered alphabetically by codename, but [pagination can be customized](https://developer.kenticocloud.com/v1/reference#listing-response).\n\nSee <https://developer.kenticocloud.com/v1/reference#list-taxonomy-groups> for more details.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "View",
      "item": [
        {
          "id": "d317eece-6fc3-44a4-ac49-60b22fab43aa",
          "name": "975bf280Fd91488c994c2f04416e5ee3TaxonomiesPersonasGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/975bf280-fd91-488c-994c-2f04416e5ee3/taxonomies/personas",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a specific taxonomy group from your project by specifying its codename.\n\nSee <https://developer.kenticocloud.com/v1/reference#view-a-taxonomy-group> for more details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "86749c8b-342a-4a04-9119-1e0f0b2e1278"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "c1bab989-8aeb-4e17-b39f-fbd29c0c30e4",
          "name": "975bf280Fd91488c994c2f04416e5ee3TaxonomiesGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/975bf280-fd91-488c-994c-2f04416e5ee3/taxonomies",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve a paginated list of taxonomy groups in your project.\n\nBy default, the API returns all taxonomy groups ordered alphabetically by codename, but [pagination can be customized](https://developer.kenticocloud.com/v1/reference#listing-response).\n\nSee <https://developer.kenticocloud.com/v1/reference#list-taxonomy-groups> for more details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c9eaad0-1b5e-4da1-a192-ea4a9963ae8e"
            }
          ]
        }
      ]
    }
  ]
}