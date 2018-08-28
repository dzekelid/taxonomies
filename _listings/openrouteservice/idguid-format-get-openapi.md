---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 0
info:
  title: AP Metadata Services Taxonomy Information
  description: Returns the taxonomy information for the specified GUID of an AP term
    and the specified format.
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---