# Airstack GraphQL API

Airstack exposes a composable GraphQL API for querying on-chain and off-chain Web3 data across multiple EVM-compatible blockchains. The API aggregates token balances, NFT metadata, token transfers, wallet identities, ENS domains, POAP attendance records, social graph data (Farcaster and Lens), and trending on-chain activity into a single unified interface. Developers can join data across chains, protocols, and identities in a single request without running indexing infrastructure themselves.

Authentication uses an API key passed as the `Authorization` header with each request. API keys are obtained from the Airstack dashboard at app.airstack.xyz. The API supports cursor-based pagination on all list queries via a `pageInfo` object that returns `nextCursor` and `prevCursor` values. Requests that access Farcaster-specific GraphQL endpoints (FarcasterCasts, FarcasterChannels, FarcasterReactions, etc.) should be noted as deprecated as of late 2024; Airstack has directed developers to use Neynar for Farcaster data going forward.

The GraphQL API supports queries across Ethereum, Base, Zora, Polygon, Degen, Gold, Ham, and STP blockchains depending on the data type. Token balance and transfer queries accept a `blockchain` enum field that selects the target chain, while social and Farcaster queries use an `EveryBlockchain` enum. The API does not expose mutations; it is a read-only data access layer.

**Endpoint:** https://api.airstack.xyz/gql

**Documentation:** https://docs.airstack.xyz/airstack-docs-and-faqs/api-capabilities

**References:**

- Documentation: https://docs.airstack.xyz/airstack-docs-and-faqs/api-capabilities
- GettingStarted: https://docs.airstack.xyz/airstack-docs-and-faqs/basics
