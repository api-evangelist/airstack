# Airstack API FinOps

## Cost Model

Airstack charges on a **per-credit** basis for production API key usage.

| Metric | Value |
|--------|-------|
| Cost per credit | $0.00002 USD |
| Billing trigger | Production key; after free credits are exhausted |
| Payment method | Credit/debit card (added during account setup) |

---

## Cost Estimation

Because credits map closely to API calls, cost estimation is straightforward:

| Monthly Calls | Estimated Cost (USD) |
|---------------|----------------------|
| 100,000 | $2.00 |
| 500,000 | $10.00 |
| 1,000,000 | $20.00 |
| 5,000,000 | $100.00 |
| 10,000,000 | $200.00 |

> Complex multi-chain or multi-project composable queries may consume more than one credit per call. Verify actual credit consumption in your Airstack dashboard.

---

## Cost Controls

- **Test Key**: No charges incurred during development/testing. Use test keys for all development and staging environments.
- **Monitor Usage**: Track credit consumption via the Airstack dashboard at [app.airstack.xyz](https://app.airstack.xyz).
- **Pagination**: Use cursor-based pagination with appropriate page sizes (default 50, max 200) to avoid fetching more data than necessary.
- **Query Optimization**: Airstack's composability lets you combine multiple data types in a single query, reducing total API calls and credit consumption vs. making separate requests.

---

## Token-Gated Access

API access requires holding the **/airstack Channel Fan Token** on Farcaster. Factor the cost of acquiring and holding this token into your overall budget. Fan Tokens are available at [airstack.xyz/channels/airstack](https://www.airstack.xyz/channels/airstack).

---

## Enterprise Pricing

For high-volume use cases requiring negotiated rates or SLAs, contact Airstack via [Telegram](https://t.me/+1k3c2FR7z51mNDRh).

---

## References

- [Get API Key](https://docs.airstack.xyz/airstack-docs-and-faqs/get-api-key)
- [Dashboard](https://app.airstack.xyz)
- [Tech Infra & Capabilities](https://docs.airstack.xyz/airstack-docs-and-faqs/api-capabilities)
