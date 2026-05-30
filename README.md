# FakerAPI (fakerapi)

FakerAPI is a free, no-authentication REST API that returns realistic fake data for developers, designers, and QA engineers. Built on top of the PHP Faker library by Alessandro Pietrantonio, it exposes a uniform set of GET endpoints for addresses, books, companies, images, persons, places, products, texts, users, and a fully custom resource builder. Every endpoint accepts the same three control parameters (`_quantity`, `_locale`, `_seed`) and returns the same envelope, making it trivial to use for prototypes, mock servers, workshop fixtures, and integration tests.

**URL:** [https://github.com/pietrantonio91/faker-api](https://github.com/pietrantonio91/faker-api)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=opensource-api-evangelist&utm_content=repo)

## Type

- **x-type:** opensource (community)
- **x-tier:** 3 (bulk-registered from public-apis, then enriched)
- **License:** Open Source (no SPDX identifier declared on the upstream repo)
- **Governance:** Single-author open source project

## Tags

- Test Data, Fake Data, Mocking, Developer Tools, Open Source, Public APIs

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### FakerAPI

Free, no-authentication REST API serving fake data across ten resource collections (addresses, books, companies, images, persons, places, products, texts, users, custom). Every operation is a GET and shares the same response envelope (`status`, `code`, `locale`, `seed`, `total`, `data`).

**Human URL:** [https://fakerapi.it/en](https://fakerapi.it/en)
**Base URL:** `https://fakerapi.it/api/v1`

#### Tags

- Test Data, Fake Data

#### Documentation

- [Documentation](https://fakerapi.it/en)
- [OpenAPI](openapi/fakerapi-openapi.yml)

#### JSON Schema

- [Address](json-schema/fakerapi-address-schema.json)
- [Book](json-schema/fakerapi-book-schema.json)
- [Company](json-schema/fakerapi-company-schema.json)
- [Envelope](json-schema/fakerapi-envelope-schema.json)
- [Image](json-schema/fakerapi-image-schema.json)
- [Person](json-schema/fakerapi-person-schema.json)
- [Place](json-schema/fakerapi-place-schema.json)
- [Product](json-schema/fakerapi-product-schema.json)
- [Text](json-schema/fakerapi-text-schema.json)
- [User](json-schema/fakerapi-user-schema.json)

#### JSON Structure

- [Address](json-structure/fakerapi-address-structure.json)
- [Book](json-structure/fakerapi-book-structure.json)
- [Company](json-structure/fakerapi-company-structure.json)
- [Envelope](json-structure/fakerapi-envelope-structure.json)
- [Image](json-structure/fakerapi-image-structure.json)
- [Person](json-structure/fakerapi-person-structure.json)
- [Place](json-structure/fakerapi-place-structure.json)
- [Product](json-structure/fakerapi-product-structure.json)
- [Text](json-structure/fakerapi-text-structure.json)
- [User](json-structure/fakerapi-user-structure.json)

#### Examples

- [List Addresses](examples/fakerapi-list-addresses-example.json)
- [List Books](examples/fakerapi-list-books-example.json)
- [List Companies](examples/fakerapi-list-companies-example.json)
- [List Custom](examples/fakerapi-list-custom-example.json)
- [List Images](examples/fakerapi-list-images-example.json)
- [List Persons](examples/fakerapi-list-persons-example.json)
- [List Places](examples/fakerapi-list-places-example.json)
- [List Products](examples/fakerapi-list-products-example.json)
- [List Texts](examples/fakerapi-list-texts-example.json)
- [List Users](examples/fakerapi-list-users-example.json)

#### Naftiko Capabilities

One self-contained capability per resource. Each file inlines its `consumes` block plus a REST exposer and an MCP exposer.

- [Addresses](capabilities/fakerapi-addresses.yaml)
- [Books](capabilities/fakerapi-books.yaml)
- [Companies](capabilities/fakerapi-companies.yaml)
- [Custom](capabilities/fakerapi-custom.yaml)
- [Images](capabilities/fakerapi-images.yaml)
- [Persons](capabilities/fakerapi-persons.yaml)
- [Places](capabilities/fakerapi-places.yaml)
- [Products](capabilities/fakerapi-products.yaml)
- [Texts](capabilities/fakerapi-texts.yaml)
- [Users](capabilities/fakerapi-users.yaml)

## Common Properties

- [Website](https://fakerapi.it/en)
- [GitHubRepository](https://github.com/pietrantonio91/faker-api)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [JSON-LD Context](json-ld/fakerapi-context.jsonld)
- [Spectral Rules](rules/fakerapi-rules.yml)
- [Vocabulary](vocabulary/fakerapi-vocabulary.yml)

## Features

| Name | Description |
|------|-------------|
| Ten Resource Collections | Addresses, books, companies, images, persons, places, products, texts, users, and a custom resource builder. |
| No Authentication | Every endpoint is open; no API key or registration required. |
| 60+ Locales | Generate data in en_US, fr_FR, it_IT, ja_JP, and 60+ other locales via the `_locale` parameter. |
| Deterministic Seeding | Pass `_seed` to make payloads exactly reproducible across runs. |
| Up to 1000 Records Per Call | Tune `_quantity` from 1 to 1000 records per request, default 10. |
| Custom Schema Endpoint | `/api/v1/custom` accepts a caller-defined field map (e.g. `name=name&email=email&phone=phoneNumber`) and returns matching records. |
| Standard Response Envelope | Every endpoint returns the same `{status, code, locale, seed, total, data}` shape. |
| Free Forever | Service is described as "Free, Forever" with no published rate limits. |

## Use Cases

| Name | Description |
|------|-------------|
| Frontend Prototyping | Populate React, Vue, or Svelte mockups with realistic data without standing up a backend. |
| API Mocking | Use FakerAPI directly or as a fixture source for Microcks, Prism, MSW, or Postman. |
| QA Test Data | Generate deterministic test fixtures (via `_seed`) for automated browser and API tests. |
| Workshop and Training Fixtures | Hand learners a single URL to fetch sample data instead of provisioning per-student accounts. |
| Database Seeding | Seed development databases with thousands of fake users, companies, or products. |
| Internationalization Testing | Exercise i18n code paths with names, addresses, and phone numbers in 60+ locales. |
| Load Test Payload Generation | Pull large, reproducible JSON payloads to feed load generators. |

## Integrations

| Name | Description |
|------|-------------|
| PHP Faker | FakerAPI is a thin HTTP wrapper over the venerable PHP Faker library by François Zaninotto. |
| Postman / Insomnia | Trivially imported as a GET-only collection. |
| Microcks / Prism / MSW | FakerAPI payloads work well as fixture sources for HTTP mocking tools. |
| Frontend Frameworks | React, Vue, Svelte, Angular, and SolidJS all fetch FakerAPI JSON directly during development. |
| Naftiko | Wrapped per-resource as Naftiko capabilities exposing REST and MCP adapters routed to fakerapi.it. |

## Notes

- The upstream repository [pietrantonio91/faker-api](https://github.com/pietrantonio91/faker-api) is the canonical source for the fakerapi.it service. It is a small JavaScript/PHP/Blade codebase by Alessandro Pietrantonio, with no published SPDX license file.
- No MCP server or Claude Code skill is published by this provider as of the enrichment date.
- No Kubernetes CRDs are produced by this project.
- No commercial / hosted offering exists — plans, rate limits, and FinOps artifacts are intentionally not generated for this FOSS provider.

## Maintainers

- **Kin Lane** — kin@apievangelist.com
