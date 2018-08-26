---
swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 0
info:
  title: Kentico Cloud View a taxonomy group
  description: |-
    Retrieve a specific taxonomy group from your project by specifying its codename.

    See <https://developer.kenticocloud.com/v1/reference#view-a-taxonomy-group> for more details.
  version: 1.0.0
host: deliver.kenticocloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /975bf280-fd91-488c-994c-2f04416e5ee3/taxonomies/personas:
    get:
      summary: View a taxonomy group
      description: |-
        Retrieve a specific taxonomy group from your project by specifying its codename.

        See <https://developer.kenticocloud.com/v1/reference#view-a-taxonomy-group> for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3TaxonomiesPersonasGet
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3taxonomiespersonas-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - View
      - Taxonomy
      - Group
  /975bf280-fd91-488c-994c-2f04416e5ee3/taxonomies:
    get:
      summary: List taxonomy groups
      description: |-
        Retrieve a paginated list of taxonomy groups in your project.

        By default, the API returns all taxonomy groups ordered alphabetically by codename, but [pagination can be customized](https://developer.kenticocloud.com/v1/reference#listing-response).

        See <https://developer.kenticocloud.com/v1/reference#list-taxonomy-groups> for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3TaxonomiesGet
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3taxonomies-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Taxonomy
      - Groups
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