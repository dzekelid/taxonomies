{
  "info": {
    "name": "AP Metadata Services Taxonomy Information",
    "_postman_id": "c2bab833-4dcd-4f5a-a9af-f498a4218046",
    "description": "Returns the taxonomy information for the specified GUID of an AP term and the specified format.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Change",
      "item": [
        {
          "id": "fd5c931a-7625-44f5-9db3-51f30f5f472d",
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
              "id": "cc78e119-de7f-4a58-a507-87e5e90db0e0"
            }
          ]
        }
      ]
    },
    {
      "name": "Ontology",
      "item": [
        {
          "id": "a0b17547-a387-4f25-a327-3469c76905f6",
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
              "id": "238808c6-26e8-4bda-aeac-f889691b73e6"
            }
          ]
        }
      ]
    },
    {
      "name": "DeprecatedCompany",
      "item": [
        {
          "id": "cb2face1-9e3e-4ba7-afdc-4bae6f651d50",
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
              "id": "7210340c-6792-498c-b644-4f0550513933"
            }
          ]
        }
      ]
    },
    {
      "name": "Deprecated",
      "item": [
        {
          "id": "020a84f7-6850-44bb-a6a3-622eac02de2d",
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
              "id": "43a075ac-5085-40e4-a6ae-07e7f0f0bb6e"
            }
          ]
        }
      ]
    },
    {
      "name": "Taxonomy",
      "item": [
        {
          "id": "76f9e2f6-a961-4d88-97af-2a02a7022c09",
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
              "id": "f6aed6c6-cbf6-4a43-bc7c-fe900c2fd3a6"
            }
          ]
        },
        {
          "id": "a4812c3d-91eb-4de4-8aec-c7175caf7849",
          "name": "getGu.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "cv.ap.org",
              "path": [
                "id/:GUID.json"
              ],
              "query": [
                {
                  "key": "apiKey",
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
                  "id": "GUID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the taxonomy information for the specified GUID of an AP term and the specified format."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3720f0c7-02ef-40aa-839f-b89b7016965f"
            }
          ]
        }
      ]
    },
    {
      "name": "Authority",
      "item": [
        {
          "id": "b18019e9-ccfb-4854-ae0f-a2ab85deef2e",
          "name": "getDAuthorityGu.Format",
          "request": {
            "url": {
              "protocol": "http",
              "host": "cv.ap.org",
              "path": [
                "d/:authority/:GUID.json"
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
                },
                {
                  "id": "GUID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a document for the specified authority and format with the AP vocabulary data for the  specified term GUID and the subset of the vocabulary located below the specified term."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80f75119-bb12-4357-8aac-54a0e348bfa0"
            }
          ]
        }
      ]
    }
  ]
}