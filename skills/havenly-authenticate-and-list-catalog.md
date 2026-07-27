---
name: Authenticate and browse the Havenly vendor catalog
description: Get an OAuth2 Bearer token, page through the vendor product catalog, resolve attribute types, and fetch user-specific data for a set of variants.
api: openapi/havenly-openapi.yml
operations: [externalOauthAuthentication, fetchVendorVariants, getUserSpecificData, fetchAttributeTypes]
---

# Authenticate and browse the Havenly vendor catalog

Use the Havenly REST API (`https://api.havenly.com`) to authenticate and read the shoppable
vendor catalog. Responses are HAL+JSON; collections paginate with `page` and `limit`.

## Steps

1. **Authenticate** — `POST /oauth` (`externalOauthAuthentication`) with a JSON body
   `{ "grant_type": "password", "username": ..., "password": ..., "client_id": ... }`.
   Read `access_token` from the response and send it on every subsequent call as
   `Authorization: Bearer <access_token>`. Tokens expire in ~3600s; use `refresh_token` to renew.
2. **List catalog** — `GET /vendor-variants?page=1&limit=5` (`fetchVendorVariants`). Read the
   collection from `_embedded`; use `page`, `page_count`, and `total_items` to iterate pages.
   Apply zf-doctrine-querybuilder filter params to narrow results.
3. **Resolve attributes** — `GET /attribute-types` (`fetchAttributeTypes`) to map attribute
   dimensions (color, material, dimensions, pattern, size, weight) referenced by variants.
4. **User-specific data** — `POST /searched-vendor-variants` (`getUserSpecificData`) with a list
   of vendor variant ids to get per-user cart/registry/opinion/purchase state and promotions.

## Rules

- Auth: all catalog reads require a valid Bearer token (unauthenticated calls return 403/401).
- Errors follow RFC 7807 (`type`, `title`, `status`, `detail`); see `errors/havenly-problem-types.yml`.
- No idempotency-key mechanism is documented; treat writes as non-idempotent and avoid blind retries.
