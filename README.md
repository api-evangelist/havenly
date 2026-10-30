# Havenly

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Havenly is an online interior-design platform that connects clients with professional designers for virtual and in-person home-decorating services. Clients take a style quiz, match with a designer, collaborate on 3D room renderings, and shop curated furniture and decor from partner brands at exclusive prices. Havenly also offers AI-assisted design. The company exposes a REST API (documented publicly via Postman at api-docs.havenly.com) covering users and profiles, addresses, design boards and board products, a vendor product catalog (vendor variants), attribute types, board feedback, and user opinions/likes. Authentication is OAuth2 (password grant) returning a Bearer token; HAL+JSON responses use page/limit pagination and zf-doctrine-querybuilder query filters. Havenly is backed by 500 Global and Foundry Group.

**Areas:** Company · Interior Design · Home Decor · Furniture · E-Commerce · Marketplace · Design · Retail · Artificial Intelligence

## Havenly on APIs.io

Everything profiled for Havenly is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/havenly/](https://apis.io/providers/havenly/)** — or go straight to one of the APIs or properties below.

### APIs (11)

- [Havenly Addresses API](https://apis.io/apis/havenly/havenly-addresses-api/) — The Addresses API from Havenly — 1 operation(s) for addresses.
- [Havenly Attribute Types API](https://apis.io/apis/havenly/havenly-attribute-types-api/) — The Attribute Types API from Havenly — 1 operation(s) for attribute types.
- [Havenly Authentication API](https://apis.io/apis/havenly/havenly-authentication-api/) — The Authentication API from Havenly — 1 operation(s) for authentication.
- [Havenly Board Feedback API](https://apis.io/apis/havenly/havenly-board-feedback-api/) — The Board Feedback API from Havenly — 2 operation(s) for board feedback.
- [Havenly Board Feedback Questions API](https://apis.io/apis/havenly/havenly-board-feedback-questions-api/) — The Board Feedback Questions API from Havenly — 2 operation(s) for board feedback questions.
- [Havenly Board Products API](https://apis.io/apis/havenly/havenly-board-products-api/) — The Board Products API from Havenly — 3 operation(s) for board products.
- [Havenly Searched Vendor Variants API](https://apis.io/apis/havenly/havenly-searched-vendor-variants-api/) — The Searched Vendor Variants API from Havenly — 1 operation(s) for searched vendor variants.
- [Havenly User Opinions API](https://apis.io/apis/havenly/havenly-user-opinions-api/) — The User Opinions API from Havenly — 2 operation(s) for user opinions.
- [Havenly User Profile API](https://apis.io/apis/havenly/havenly-user-profile-api/) — The User Profile API from Havenly — 2 operation(s) for user profile.
- [Havenly Users API](https://apis.io/apis/havenly/havenly-users-api/) — The Users API from Havenly — 1 operation(s) for users.
- [Havenly Vendor Variants API](https://apis.io/apis/havenly/havenly-vendor-variants-api/) — The Vendor Variants API from Havenly — 1 operation(s) for vendor variants.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [havenly](https://apis.io/servers/havenly/havenly/)

#### Collections (12)

Postman and Open Collection request collections.

- [Havenly Addresses API](https://apis.io/collections/havenly/open-havenly-addresses-api/)
- [Havenly Addresses Attribute Types API](https://apis.io/collections/havenly/open-havenly-attribute-types-api/)
- [Havenly Addresses Authentication API](https://apis.io/collections/havenly/open-havenly-authentication-api/)
- [Havenly Addresses Board Feedback API](https://apis.io/collections/havenly/open-havenly-board-feedback-api/)
- [Havenly Addresses Board Feedback Questions API](https://apis.io/collections/havenly/open-havenly-board-feedback-questions-api/)
- [Havenly Addresses Board Products API](https://apis.io/collections/havenly/open-havenly-board-products-api/)
- [Havenly Addresses Searched Vendor Variants API](https://apis.io/collections/havenly/open-havenly-searched-vendor-variants-api/)
- [Havenly Addresses User Opinions API](https://apis.io/collections/havenly/open-havenly-user-opinions-api/)
- [Havenly Addresses User Profile API](https://apis.io/collections/havenly/open-havenly-user-profile-api/)
- [Havenly Addresses Users API](https://apis.io/collections/havenly/open-havenly-users-api/)
- [Havenly Addresses Vendor Variants API](https://apis.io/collections/havenly/open-havenly-vendor-variants-api/)
- [Havenly API](https://apis.io/collections/havenly/postman-havenly-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Havenly Openapi Overlay](https://apis.io/overlays/havenly/havenly-openapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Havenly Authentication](https://apis.io/security/havenly/havenly-authentication/)
- [Havenly Domain Security](https://apis.io/security/havenly/havenly-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Havenly Scopes](https://apis.io/scopes/havenly/havenly-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://havenly.com)
- [Documentation](https://api-docs.havenly.com/)
- [API reference](https://api-docs.havenly.com/)
- [Pricing](https://havenly.com/pricing)
- [Sign up](https://havenly.com/interior-design-style-quiz/style-inspiration)
- [Support](https://havenly.kustomer.help)
- [Blog](https://havenly.com/blog)
- [Terms of service](https://havenly.com/terms)
- [Privacy policy](https://havenly.com/privacy)

## API Evangelist rating

**Kin Score 36.9** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 47.3 |
| Contract governance | 0.0 |
| Operational transparency | 0.0 |
| Developer ergonomics | 38.7 |
| Access clarity | 44.7 |

**Agent readiness 22.1** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | verified |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 27.3** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/havenly/](https://apis.io/providers/havenly/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Havenly: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/havenly/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
