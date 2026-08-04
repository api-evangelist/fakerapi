# FakerAPI (fakerapi)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

FakerAPI is a free, no-authentication REST API that returns realistic fake data for developers, designers, and QA engineers. Built on top of the PHP Faker library by Alessandro Pietrantonio, it exposes a uniform set of GET endpoints for addresses, books, companies, images, persons, places, products, texts, users, and a fully custom resource builder. Every endpoint accepts the same three control parameters (_quantity, _locale, _seed) and returns the same envelope, making it trivial to use for prototypes, mock servers, workshop fixtures, and integration tests.

**APIs.json:** [https://github.com/pietrantonio91/faker-api](https://github.com/pietrantonio91/faker-api)

## Tags

- Test Data
- Fake Data
- Mocking
- Developer Tools
- Open Source
- Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### FakerAPI

Free, no-authentication REST API serving fake data across ten resource collections (addresses, books, companies, images, persons, places, products, texts, users, custom). Every operation is a GET and shares the same response envelope (status, code, locale, seed, total, data).

- **Human URL:** [https://fakerapi.it/en](https://fakerapi.it/en)
- **Base URL:** `https://fakerapi.it/api/v1`

#### Tags

- Test Data
- Fake Data

#### Properties

- [Documentation](https://fakerapi.it/en)
- [OpenAPI](openapi/fakerapi-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fakerapi.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fakerapi.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/fakerapi-address-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fakerapi-book-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fakerapi-company-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fakerapi-envelope-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fakerapi-image-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fakerapi-person-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fakerapi-place-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fakerapi-product-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fakerapi-text-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/fakerapi-user-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/fakerapi-address-structure.json)
- [JSON Structure](json-structure/fakerapi-book-structure.json)
- [JSON Structure](json-structure/fakerapi-company-structure.json)
- [JSON Structure](json-structure/fakerapi-envelope-structure.json)
- [JSON Structure](json-structure/fakerapi-image-structure.json)
- [JSON Structure](json-structure/fakerapi-person-structure.json)
- [JSON Structure](json-structure/fakerapi-place-structure.json)
- [JSON Structure](json-structure/fakerapi-product-structure.json)
- [JSON Structure](json-structure/fakerapi-text-structure.json)
- [JSON Structure](json-structure/fakerapi-user-structure.json)
- [Example](examples/fakerapi-list-addresses-example.json)
- [Example](examples/fakerapi-list-books-example.json)
- [Example](examples/fakerapi-list-companies-example.json)
- [Example](examples/fakerapi-list-custom-example.json)
- [Example](examples/fakerapi-list-images-example.json)
- [Example](examples/fakerapi-list-persons-example.json)
- [Example](examples/fakerapi-list-places-example.json)
- [Example](examples/fakerapi-list-products-example.json)
- [Example](examples/fakerapi-list-texts-example.json)
- [Example](examples/fakerapi-list-users-example.json)

## Common Properties

- [Website](https://fakerapi.it/en)
- [GitHub Repository](https://github.com/pietrantonio91/faker-api)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [JSON-LD](json-ld/fakerapi-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Spectral Rules](rules/fakerapi-rules.yml)
- [Vocabulary](vocabulary/fakerapi-vocabulary.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
