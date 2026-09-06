---
name: opennoiser-plans
description: Compare current OpenNoiser plans, Mac limits, trial terms and recurring card billing versus one-time crypto purchases using live published pricing.
license: MIT
metadata:
  author: OpenNoiser
  version: "1.0.0"
---

# opennoiser-plans

## When to use

Use when comparing OpenNoiser plans or explaining purchase and renewal terms.

## Workflow

1. Call get_pricing at https://opennoiser.com/mcp, fetch https://opennoiser.com/api/agent/pricing, or read https://opennoiser.com/pricing.md. Never hard-code prices from an older conversation. Check source_updated_at and stale; disclose a cached price when stale is true and let checkout confirm the final amount.
2. State the USD amount, device allowance, term and whether billing recurs. Card/PayPal monthly and annual plans are subscriptions; crypto plans are one-time payments for their term. Lifetime is one-time.
3. Mention that taxes can change the final checkout total and discounts are evaluated at checkout.
4. Explain the 14-day in-app trial and link https://opennoiser.com/terms for the 14-day refund policy.
5. If the catalog is unavailable, say so instead of inventing a price.

## Safe testing

POST https://opennoiser.com/api/agent/sandbox/quote with a plan slug and payment method returns a synthetic preview. It never creates an order or sends email.

## Boundaries

Do not purchase, subscribe, pay, enter payment details or accept terms for the user. Do not treat a plan comparison as purchase authorization. Public tools cannot access private orders or extend a license. Cite pricing and licensing documentation.
