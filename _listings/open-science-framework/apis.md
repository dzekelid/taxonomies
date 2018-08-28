---
name: Open Science Framework
x-slug: open-science-framework
description: OSF provides free and open source project management support for researchers
  across the entire research lifecycle. As a collaboration tool, OSF helps researchers
  work on projects privately with a limited number of collaborators and make parts
  of their projects public, or make all the project publicly accessible for broader
  dissemination. As a workflow system, OSF enables connections to the many services
  researchers already use to streamline their process and increase efficiency. As
  a flexible repository, it can store and archive research data, protocols, and materials.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Taxonomies
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/taxonomies/master/_listings/open-science-framework/apis.md
specificationVersion: "0.14"
apis:
- name: Open Science Framework - List all taxonomies
  x-api-slug: preprint-providerspreprint-provider-idtaxonomies-get
  description: |-
    A paginated list of the taxonomies for a preprint provider. The returned preprint providers taxonomies are sorted by their creation date, with the most recent preprints appearing first.
    #### Returns
    Returns a JSON object containing `data` and `links` keys.

    The `data` key contains an array of 10 preprint providers. Each resource in the array is a separate preprint provider object.

    The `links` key contains a dictionary of links that can be used for [pagination](#Introduction_pagination).

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/taxonomies/master/_listings/open-science-framework/preprint-providerspreprint-provider-idtaxonomies-get-openapi.md
- name: Open Science Framework - List all taxonomies
  x-api-slug: taxonomies-get
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
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/taxonomies/master/_listings/open-science-framework/taxonomies-get-openapi.md
- name: Open Science Framework - Retrieve a taxonomy
  x-api-slug: taxonomiestaxonomy-id-get
  description: |-
    Retrieves the details of a taxonomy.
    #### Returns

    Returns a JSON object with a `data` key containing the representation of the requested taxonomy, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/taxonomies/master/_listings/open-science-framework/taxonomiestaxonomy-id-get-openapi.md
- name: Open Science Framework - Retrieve a taxonomy
  x-api-slug: taxonomiestaxonomy-id-get
  description: |-
    Retrieves the details of a taxonomy.
    #### Returns

    Returns a JSON object with a `data` key containing the representation of the requested taxonomy, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/taxonomies/master/_listings/open-science-framework/taxonomiestaxonomy-id-get-openapi.md
- name: Open Science Framework - Retrieve a taxonomy
  x-api-slug: taxonomiestaxonomy-id-get
  description: |-
    Retrieves the details of a taxonomy.
    #### Returns

    Returns a JSON object with a `data` key containing the representation of the requested taxonomy, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/taxonomies/master/_listings/open-science-framework/taxonomiestaxonomy-id-get-openapi.md
- name: Open Science Framework - Retrieve a taxonomy
  x-api-slug: taxonomiestaxonomy-id-get
  description: |-
    Retrieves the details of a taxonomy.
    #### Returns

    Returns a JSON object with a `data` key containing the representation of the requested taxonomy, if the request is successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  image: ""
  humanURL: https://cos.io
  baseURL: https://test-api.osf.io//v2
  tags: Research, Science, API Provider, Profiles, General Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/taxonomies/master/_listings/open-science-framework/taxonomiestaxonomy-id-get-openapi.md
x-common:
- type: x-website
  url: https://cos.io
- type: x-api-gallery
  url: http://open.fintech.api.gallery.streamdata.io
- type: x-api-stack
  url: http://open.science.framework.stack.network
- type: x-github
  url: https://github.com/OSFramework
- type: x-twitter
  url: https://twitter.com/OSFramework
- type: x-website
  url: http://osf.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---