# Airstack

Airstack is a Web3 data aggregation platform providing GraphQL and REST APIs for querying on-chain and off-chain data across multiple blockchains. Developers can query NFT ownership, token balances, wallet identities, ENS names, POAP badges, and cross-chain data in a single composable request.

## APIs

| API | Type | Endpoint |
|-----|------|----------|
| Airstack GraphQL API | GraphQL | `https://api.airstack.xyz/graphql` |
| Farcaster Hub API | REST / gRPC | `https://api.airstack.xyz` (deprecated) |

## Supported Data Types

- ERC20 token balances and transfers
- ERC721 / ERC1155 NFT ownership and metadata
- ERC6551 token-bound accounts
- ENS names and reverse resolution
- POAP badges
- Wallet identity resolution (cross-chain)
- Social graph data (Farcaster, Lens — Farcaster deprecated as of late 2024)
- XMTP messaging eligibility

## Supported Blockchains

- Ethereum
- Polygon
- Base
- Other EVM-compatible chains

## Authentication

Pass your Airstack API key in the `Authorization` header. A production key requires:

1. An Airstack account at [app.airstack.xyz](https://app.airstack.xyz)
2. At least 1 /airstack Channel Fan Token in a connected Farcaster wallet
3. A payment card on file

## Rate Limits

- 3,000 requests/minute
- 300 requests/second (burst)
- Maximum 200 records per query; default 50

## Pricing

$0.00002 USD per API credit. Test keys are free; production keys are billed after free credits are exhausted.

## SDKs

- [Web SDK (JS/TS)](https://github.com/Airstack-xyz/airstack-web-sdk)
- [Node.js SDK](https://github.com/Airstack-xyz/airstack-node-sdk)
- [Python SDK](https://github.com/Airstack-xyz/airstack-python-sdk)
- [Frames SDK](https://github.com/Airstack-xyz/airstack-frames-sdk)

## Resources

- [Documentation](https://docs.airstack.xyz/)
- [Explorer](https://explorer.airstack.xyz)
- [Dashboard](https://app.airstack.xyz)
- [Blog](https://blog.airstack.xyz)
- [GitHub](https://github.com/Airstack-xyz)
- [Telegram Support](https://t.me/+1k3c2FR7z51mNDRh)

## Notes

Airstack deprecated all Farcaster-related GraphQL APIs in late 2024. Developers using Farcaster data should migrate to [Neynar](https://neynar.com/). Moxie-related data is available at [developer.moxie.xyz](https://developer.moxie.xyz).

Additionally, as of 2025, the airstack.xyz domain redirects to [senpi.ai](https://www.senpi.ai/), which is a separate AI trading agent platform for Hyperliquid. The Airstack developer documentation remains at [docs.airstack.xyz](https://docs.airstack.xyz/).
