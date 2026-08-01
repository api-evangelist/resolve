---
name: Onboard a customer for net terms
description: Create a buyer, run a credit check, and enroll them in Resolve net terms.
api: openapi/resolve-merchant-api-openapi.yaml
operations: [createCustomer, requestCustomerCreditCheck, fetchCustomer, enroll-a-customer]
---

# Onboard a customer for net terms

Use the Resolve Merchant API to take a new buyer from creation through credit
underwriting to enrollment in net terms.

## Auth
Authenticate with HTTP Basic (merchant_id : secret key) or a JWT bearer token
minted from an OAuth access key (`merchant:write` scope). Base URL:
`https://app.resolvepay.com/api` (production) or
`https://app-sandbox.resolvepay.com/api` (sandbox).

## Steps
1. **createCustomer** — `POST /customers` with the buyer's business details.
   Capture the returned `customer_id`.
2. **requestCustomerCreditCheck** — `POST /customers/{customer_id}/credit-check`
   to submit the buyer for underwriting. A `400 invalid_request` with
   `Credit check already created for this customer` means a check already exists.
3. **fetchCustomer** — `GET /customers/{customer_id}`; poll credit status /
   available credit until a decision lands (also delivered via the
   `customer.credit_decision_created` / `customer.status_updated` webhooks).
4. **enroll-a-customer** — `POST /customers/{customer_id}/enroll` once approved.

## Conventions
- Errors use `{ error: { type, message, details[] } }` (see errors/resolve-problem-types.yml).
- Rate limit: 100 req/min (sliding window); honor `X-Ratelimit-*` headers, back off on 429.
- Prefer webhooks over polling for credit decisions (asyncapi/resolve-webhooks.yml).
