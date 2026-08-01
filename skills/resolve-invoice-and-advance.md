---
name: Create, send, and advance an invoice
description: Create an invoice for an enrolled customer, send it, and capture payment/advance.
api: openapi/resolve-merchant-api-openapi.yaml
operations: [createInvoice, updateInvoice, sendInvoice, fetchInvoice, createShipment]
---

# Create, send, and advance an invoice

Issue a net-terms invoice to an enrolled Resolve customer and take it through
send and fulfillment.

## Auth
JWT bearer (OAuth access key, `merchant:write`) or HTTP Basic. Base URL
`https://app.resolvepay.com/api`.

## Steps
1. **createInvoice** — `POST /invoices` for the target `customer_id` with line
   items and amount. Capture `invoice_id`.
2. **updateInvoice** — `PUT /invoices/{invoice_id}` to set `terms` and
   `advance_requested` before sending (only while the invoice is a draft).
3. **sendInvoice** — `PUT /invoices/{invoice_id}/send` to deliver it to the buyer.
4. **createShipment** — `POST /shipments` to attach tracking (courier +
   tracking number) once fulfilled.
5. **fetchInvoice** — `GET /invoices/{invoice_id}` to track balance; the
   `invoice.balance_updated` webhook fires as payments apply.

## Conventions
- Capture operations accept an `idempotency_key` in the body — always send a
  stable key to make retries safe (conventions/resolve-conventions.yml).
- Pagination on list endpoints: `limit` + `page`, response `count` + `results`.
- Void with `voidInvoice`, cancel with `cancelInvoice`; delete only unsent drafts.
