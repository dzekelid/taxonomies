---
swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 0
info:
  title: Open Science Framework Retrieve a taxonomy
  description: |-
    Retrieves the details of a taxonomy.
    #### Returns

    Returns a JSON object with a `data` key containing the representation of the requested taxonomy, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  contact:
    name: OSF
    url: https://osf.io/support
    email: support@osf.io
  version: "2.0"
host: test-api.osf.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /preprint_providers/{preprint_provider_id}/taxonomies/:
    get:
      summary: List all taxonomies
      description: |-
        A paginated list of the taxonomies for a preprint provider. The returned preprint providers taxonomies are sorted by their creation date, with the most recent preprints appearing first.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of 10 preprint providers. Each resource in the array is a separate preprint provider object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: preprint_provider_taxonomies_list
      x-api-path-slug: preprint-providerspreprint-provider-idtaxonomies-get
      parameters:
      - in: path
        name: preprint_provider_id
        description: The unique identifier of the preprint provider
      responses:
        200:
          description: OK
      tags:
      - Preprint
      - Providers
      - Preprint
      - Provider
      - Taxonomies
  /taxonomies/:
    get:
      summary: List all taxonomies
      description: |-
        A paginated list of all [bepress disciplines taxonomies](https://www.bepress.com/wp-content/uploads/2016/12/Digital-Commons-Disciplines-taxonomy-2017-01.pdf).
        Note: this API endpoint is under active development, and is subject to change in the future.
        #### Returns
        Returns a JSON object containing `data` and `links` keys.

        The `data` key contains an array of up to 10 taxonomies. Each resource in the array is a separate taxonomy object.

        The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

        This request should never return an error.
        #### Filtering
        You can optionally request that the response only include taxonomies that match your filters by utilizing the `filter` query parameter, e.g. https://api.osf.io/v2/taxonomies/?filter['id']='{taxonomy_id}'.

        Taxonomies may be filtered by their `id`, `parents`, and `text`.
      operationId: taxonomies_list
      x-api-path-slug: taxonomies-get
      responses:
        200:
          description: OK
      tags:
      - Taxonomies
  /taxonomies/{taxonomy_id}/:
    get:
      summary: Retrieve a taxonomy
      description: |-
        Retrieves the details of a taxonomy.
        #### Returns

        Returns a JSON object with a `data` key containing the representation of the requested taxonomy, if the request is successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: taxonomies_read
      x-api-path-slug: taxonomiestaxonomy-id-get
      parameters:
      - in: path
        name: taxonomy_id
        description: The unique identifier of the taxonomy
      responses:
        200:
          description: OK
      tags:
      - Taxonomies
      - Taxonomy
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