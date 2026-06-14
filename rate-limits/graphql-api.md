# Airstack GraphQL API Rate Limits

## Rate Limits

| Limit Type | Value |
|------------|-------|
| Requests per minute | 3,000 |
| Burst (requests per second) | 300 |

These limits apply to all API keys. Contact Airstack via [Telegram](https://t.me/+1k3c2FR7z51mNDRh) if you require higher throughput.

---

## Query Limits

| Parameter | Value |
|-----------|-------|
| Maximum records per API call | 200 |
| Default records per API call | 50 |
| Maximum array length for `_in` / `_nin` filters | 200 items |

Pagination is cursor-based. Use the `pageInfo.nextCursor` field in responses to retrieve subsequent pages.

---

## Endpoint

```
POST https://api.airstack.xyz/graphql
```

### Required Headers

| Header | Value |
|--------|-------|
| `Authorization` | Your Airstack API key |
| `Content-Type` | `application/json` (when using REST-style POST) |

---

## Authentication Notes

The API key is passed in the `Authorization` header (not as `Bearer <token>` — just the raw key value).

---

## References

- [Tech Infra & Capabilities](https://docs.airstack.xyz/airstack-docs-and-faqs/api-capabilities)
- [Direct API Call Guide](https://docs.airstack.xyz/airstack-docs-and-faqs/basics)
- [Get API Key](https://docs.airstack.xyz/airstack-docs-and-faqs/get-api-key)
