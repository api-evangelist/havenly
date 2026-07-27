---
name: Add a vendor product to a design board
description: Authenticate, find a vendor variant, add it to a design board as a board product, then read the board product back.
api: openapi/havenly-openapi.yml
operations: [externalOauthAuthentication, fetchVendorVariants, createBoardProduct, getASpecificBoardProductById]
---

# Add a vendor product to a design board

Place a catalog product onto a Havenly design board. Base URL `https://api.havenly.com`.

## Steps

1. **Authenticate** — `POST /oauth` (`externalOauthAuthentication`); capture `access_token` and
   send `Authorization: Bearer <access_token>` on all following calls.
2. **Find the product** — `GET /vendor-variants?page=1&limit=5` (`fetchVendorVariants`) to locate
   the `vendorVariant` id you want to place.
3. **Add to board** — `POST /board-products` (`createBoardProduct`) with a JSON body linking the
   board and the variant, e.g. `{ "recommendedQty": 5, "board": <boardId>, "vendorVariant": <variantId>, "status": 2 }`.
   A `201 Created` returns the new board product.
4. **Read it back** — `GET /board-products/{id}` (`getASpecificBoardProductById`) for the full
   HAL representation, or `GET /board-products-lite/{id}` for a lighter payload.

## Rules

- All operations require a valid Bearer token; a missing/invalid token returns 401/403.
- Requests and responses are JSON / HAL+JSON; see `conventions/havenly-conventions.yml`.
- Errors follow RFC 7807; see `errors/havenly-problem-types.yml`.
- No documented idempotency key — do not blindly retry `createBoardProduct` on timeout; read
  back the board first to avoid duplicates.
