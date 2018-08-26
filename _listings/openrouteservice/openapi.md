---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 1
info:
  title: AP Metadata Services
  description: add-value-to-your-news-content-with-apu2019s-industryleading-metadata--accurate-comprehensive-richly-detailed-data-designed-specifically-for-use-by-news-publishers--ap-metadata-services-is-a-new-set-of-apis-that-gives-you-direct-access-to-the-same-metadata-system-that-supports-apu2019s-awardwinning-global-news-operation-
  version: v1
host: cv.ap.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  d/{authority}.{format}:
    get:
      summary: Taxonomy Information
      description: Returns the taxonomy information for the specified authority and
        the specified format.
      operationId: getDAuthority.Format
      x-api-path-slug: dauthority-format-get
      parameters:
      - in: query
        name: apikey
        description: API Key
      - in: path
        name: authority
        description: The name of a classification authority (not case-sensitive)
      - in: path
        name: format
        description: The format of the returned taxonomy data
      responses:
        200:
          description: OK
      tags:
      - Taxonomy
      - Information
  id/{GUID}.{format}:
    get:
      summary: Taxonomy Information
      description: Returns the taxonomy information for the specified GUID of an AP
        term and the specified format.
      operationId: getGu.Format
      x-api-path-slug: idguid-format-get
      parameters:
      - in: query
        name: apiKey
        description: API Key
      - in: path
        name: format
        description: The format of the returned taxonomy data
      - in: path
        name: GUID
        description: The GUID of an AP term (not case-sensitive)
      responses:
        200:
          description: OK
      tags:
      - Taxonomy
      - Information
---