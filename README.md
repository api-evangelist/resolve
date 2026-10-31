# Resolve

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

Resolve is a B2B commerce and payments platform that lets businesses offer flexible net terms (typically NET 30-60) to their buyers without carrying the credit risk or waiting on cash. It combines automated credit underwriting, invoicing, agentic collections, and payment processing: sellers are paid upfront while customers pay on terms. Resolve exposes a Merchant API (V5) for direct integrations (customers, credit checks, invoices, orders, charges, shipments, payments, payouts), a Partners API for platform/marketplace sub-merchant management, a browser Checkout SDK, and an official MCP server with full Merchant-API parity for AI assistants. Backed by Insight Partners, QED Investors, and Y Combinator.

**Areas:** Company · Payments · B2B · Net Terms · Credit · Invoicing · Financing · Embedded Finance

## Resolve on APIs.io

Everything profiled for Resolve is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/resolve/](https://apis.io/providers/resolve/)** — or go straight to one of the APIs or properties below.

### APIs (12)

- [Resolve Access Keys API](https://apis.io/apis/resolve/resolve-access-keys-api/) — OAuth access keys are created in Merchant Dashboard and can be exchanged for bearer tokens. Use the `/access-keys/token` endpoint to mint a bearer token…
- [Resolve Charges API](https://apis.io/apis/resolve/resolve-charges-api/) — A charge represents an agreement by the customer to accept credit terms for a transaction. It consists of a charge amount, term length (i.e. 30, 60, 90),…
- [Resolve Credit Notes API](https://apis.io/apis/resolve/resolve-credit-notes-api/) — Credit Notes are issued to customers to reduce the amount they owe.
- [Resolve Customers API](https://apis.io/apis/resolve/resolve-customers-api/) — A customer represents a company that you do business with. For larger companies, there may be several users with access to the customer account that can…
- [Resolve Invoices API](https://apis.io/apis/resolve/resolve-invoices-api/) — The invoice represents the business transaction between you and your customer. In Resolve, an invoice must be tied to a customer and an advance can be taken…
- [Resolve Merchants API](https://apis.io/apis/resolve/resolve-merchants-api/) — Merchant-scoped operations for managing sub-merchant resources. The merchant document upload endpoint creates a document record and starts transfer into…
- [Resolve Orders API](https://apis.io/apis/resolve/resolve-orders-api/) — An order represents an authorization of credit for a customer transaction. Once authorized, an order can be partially or fully captured as goods or services…
- [Resolve Payments API](https://apis.io/apis/resolve/resolve-payments-api/) — A payment represents a transaction where a customer pays towards their invoices. When a payment is made to Resolve, the customer's available credit balance…
- [Resolve Payout Transactions API](https://apis.io/apis/resolve/resolve-payout-transactions-api/) — Payout Transactions are the individual transactions like customer payments, Resolve advances, forwarded payments, etc. that are rolled into a Payout. Each…
- [Resolve Payouts API](https://apis.io/apis/resolve/resolve-payouts-api/) — A Payout is a transfer of money between the Merchant and Resolve.
- [Resolve Shipments API](https://apis.io/apis/resolve/resolve-shipments-api/) — A shipment represents the fulfillment of goods or services for an invoice. Track shipments to monitor delivery status and fulfillment progress. Shipments…
- [Resolve Webhooks API](https://apis.io/apis/resolve/resolve-webhooks-api/) — Webhooks allow you to receive real-time notifications about events in your Resolve account. When an event occurs, Resolve sends an HTTP POST request to your…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Resolve Webhooks](https://apis.io/asyncapis/resolve/resolve-webhooks/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [resolve](https://apis.io/servers/resolve/resolve/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Resolve Agentic Access](https://apis.io/agentic-access/resolve/resolve-agentic-access/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Resolve Context](https://apis.io/jsonld/resolve/resolve-context/)

#### Collections (24)

Postman and Open Collection request collections.

- [Resolve API Reference Access Keys API](https://apis.io/collections/resolve/open-resolve-access-keys-api/)
- [Resolve API Reference Access Keys Charges API](https://apis.io/collections/resolve/open-resolve-charges-api/)
- [Resolve API Reference Access Keys Credit Notes API](https://apis.io/collections/resolve/open-resolve-credit-notes-api/)
- [Resolve API Reference Access Keys Customers API](https://apis.io/collections/resolve/open-resolve-customers-api/)
- [Resolve API Reference Access Keys Invoices API](https://apis.io/collections/resolve/open-resolve-invoices-api/)
- [Resolve API Reference Access Keys Merchants API](https://apis.io/collections/resolve/open-resolve-merchants-api/)
- [Resolve API Reference Access Keys Orders API](https://apis.io/collections/resolve/open-resolve-orders-api/)
- [Resolve API Reference Access Keys Payments API](https://apis.io/collections/resolve/open-resolve-payments-api/)
- [Resolve API Reference Access Keys Payout Transactions API](https://apis.io/collections/resolve/open-resolve-payout-transactions-api/)
- [Resolve API Reference Access Keys Payouts API](https://apis.io/collections/resolve/open-resolve-payouts-api/)
- [Resolve API Reference Access Keys Shipments API](https://apis.io/collections/resolve/open-resolve-shipments-api/)
- [Resolve API Reference Access Keys Webhooks API](https://apis.io/collections/resolve/open-resolve-webhooks-api/)
- [Resolve API Reference Access Keys API](https://apis.io/collections/resolve/postman-resolve-access-keys-api/)
- [Resolve API Reference Access Keys Charges API](https://apis.io/collections/resolve/postman-resolve-charges-api/)
- [Resolve API Reference Access Keys Credit Notes API](https://apis.io/collections/resolve/postman-resolve-credit-notes-api/)
- [Resolve API Reference Access Keys Customers API](https://apis.io/collections/resolve/postman-resolve-customers-api/)
- [Resolve API Reference Access Keys Invoices API](https://apis.io/collections/resolve/postman-resolve-invoices-api/)
- [Resolve API Reference Access Keys Merchants API](https://apis.io/collections/resolve/postman-resolve-merchants-api/)
- [Resolve API Reference Access Keys Orders API](https://apis.io/collections/resolve/postman-resolve-orders-api/)
- [Resolve API Reference Access Keys Payments API](https://apis.io/collections/resolve/postman-resolve-payments-api/)
- [Resolve API Reference Access Keys Payout Transactions API](https://apis.io/collections/resolve/postman-resolve-payout-transactions-api/)
- [Resolve API Reference Access Keys Payouts API](https://apis.io/collections/resolve/postman-resolve-payouts-api/)
- [Resolve API Reference Access Keys Shipments API](https://apis.io/collections/resolve/postman-resolve-shipments-api/)
- [Resolve API Reference Access Keys Webhooks API](https://apis.io/collections/resolve/postman-resolve-webhooks-api/)

#### Overlays (2)

OpenAPI overlays, including conversational phrasing for each operation.

- [Resolve Merchant Api Overlay](https://apis.io/overlays/resolve/resolve-merchant-api-overlay/)
- [Resolve Partners Api Overlay](https://apis.io/overlays/resolve/resolve-partners-api-overlay/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Resolve API Rules](https://apis.io/rules/resolve/resolve-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Resolve Authentication](https://apis.io/security/resolve/resolve-authentication/)
- [Resolve Domain Security](https://apis.io/security/resolve/resolve-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Resolve Scopes](https://apis.io/scopes/resolve/resolve-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Resolve Plans Pricing](https://apis.io/plans/resolve/resolve-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Resolve Rate Limits](https://apis.io/rate-limits/resolve/resolve-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://resolvepay.com/)
- [Documentation](https://docs.resolvepay.com)
- [Getting started](https://docs.resolvepay.com/guides)
- [API reference](https://docs.resolvepay.com/api-reference)
- [Pricing](https://resolvepay.com/pricing/)
- [Sign up](https://resolvepay.com/signup/)
- [Support](https://help.resolvepay.com/)
- [Blog](https://resolvepay.com/blog)
- [Trust centre](https://trust.resolvepay.com)
- [Terms of service](https://resolvepay.com/terms/)
- [Privacy policy](https://resolvepay.com/privacy/)
- [GitHub](https://github.com/resolvepay)
- [Status](https://status.resolvepay.com)

## API Evangelist rating

**Kin Score 67.6** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 66.1 |
| Contract governance | 22.0 |
| Operational transparency | 55.3 |
| Developer ergonomics | 67.3 |
| Access clarity | 65.8 |

**Agent readiness 65.8** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | verified |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | verified |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | paginated |
| Operation Distinctiveness | distinct |

**Regulatory alignment 31.3** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/resolve/](https://apis.io/providers/resolve/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Resolve: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/resolve/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
