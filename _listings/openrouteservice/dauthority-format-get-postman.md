{
  "info": {
    "name": "AP Metadata Services Taxonomy Information",
    "_postman_id": "171b8a66-446e-4045-ba97-f99b68086f64",
    "description": "Returns the taxonomy information for the specified authority and the specified format.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Change",
      "item": [
        {
          "id": "6edd6693-328e-4a4b-b7dd-78c4a9a0df27",
          "name": "getApiCm",
          "request": {
            "url": "http://cv.ap.org/api/cm/?apiKey=%7B%7D&authority=%7B%7D&enddate=%7B%7D&format=%7B%7D&lastversion=%7B%7D&startdate=%7B%7D&version=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of changes to the AP vocabulary terms according to the specified criteria."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5431a053-3b64-45c7-b558-f2d8a998feb4"
            }
          ]
        }
      ]
    },
    {
      "name": "Ontology",
      "item": [
        {
          "id": "911078a3-694e-42b5-b09d-a5c5531ab5ca",
          "name": "getCClass.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "cv.ap.org",
              "path": [
                "c/:class.json"
              ],
              "query": [
                {
                  "key": "apikey",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "class",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the AP ontology definition for the specified AP property or class and the specified format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b877d3d-d2d5-4256-95ea-b9daa52c0183"
            }
          ]
        }
      ]
    },
    {
      "name": "DeprecatedCompany",
      "item": [
        {
          "id": "f5590485-14da-49c5-8484-f055c1528417",
          "name": "getDDeprecatedcompany.Format",
          "request": {
            "url": "http://cv.ap.org/d/DeprecatedCompany.json?apiKey=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of deprecated AP vocabulary terms in the specified format for the AP Company authority  or for the other four AP authorities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bf777dd-f2e6-4ef9-bee5-a4b8db9a2f99"
            }
          ]
        }
      ]
    },
    {
      "name": "Deprecated",
      "item": [
        {
          "id": "1b4e5a63-43b5-4369-8617-53c6c68c797d",
          "name": "getDDeprecatedterm.Format",
          "request": {
            "url": "http://cv.ap.org/d/DeprecatedTerm.json?apiKey=%7B%7D&format=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of deprecated AP vocabulary terms in the specified format for the AP Company authority  or for the other four AP authorities."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b807ef5-6efb-4b92-a4c3-bf59ae15631e"
            }
          ]
        }
      ]
    },
    {
      "name": "Taxonomy",
      "item": [
        {
          "id": "c3b9038f-455e-4fc5-8dab-114196c19ffa",
          "name": "getDAuthority.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "cv.ap.org",
              "path": [
                "d/:authority.json"
              ],
              "query": [
                {
                  "key": "apikey",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "authority",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the taxonomy information for the specified authority and the specified format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1f97e2b-70b6-424a-9253-4cbf920e9a03"
            }
          ]
        }
      ]
    }
  ]
}