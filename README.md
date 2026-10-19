# Awesome Ophis [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Integration surfaces, examples, and tools for [Ophis](https://ophis.fi) — an intent-based, MEV-protected DEX (a CoW Protocol fork) live on 11 EVM chains, with natural-language and AI-agent swaps via an MCP server and a TypeScript SDK.

Ophis settles every trade through CoW Protocol's batch auction, so trades are MEV-protected and gasless, with price-improvement surplus returned to the trader. Integrators embed swaps and earn a referral rebate (8 to 12 percent of the net fee) on their users' volume.

## Contents
- [Start here](#start-here)
- [SDK](#sdk)
- [MCP server (AI agents)](#mcp-server-ai-agents)
- [Ophis CLI](#ophis-cli)
- [Widget](#widget)
- [Examples](#examples)
- [Chains](#chains)
- [Earn (referral rebate)](#earn-referral-rebate)
- [Links](#links)

## Start here
- [ophis.fi](https://ophis.fi) — the app
- [swap.ophis.fi](https://swap.ophis.fi) — the swap UI (embeddable)
- [docs.ophis.fi](https://docs.ophis.fi) — documentation
- [github.com/ophis-fi/ophis](https://github.com/ophis-fi/ophis) — the protocol monorepo

## SDK
`@ophis/sdk` is the integration path that carries your referral code, so the rebate is attributed to you.
- npm: [`@ophis/sdk`](https://www.npmjs.com/package/@ophis/sdk)
- Helpers: correct orderbook hosts per chain, the CIP-75 partner-fee appData fragment, the per-chain EIP-712 signing domain, and order receiver-safety guards.

## MCP server (AI agents)
A Model Context Protocol server that gives any agent a swap tool (quote, build, sign, status) over the same 11 chains.
- Hosted endpoint + per-client setup: see [docs.ophis.fi](https://docs.ophis.fi)
- Works with Claude Desktop, Cursor, Cline, Goose, and any MCP client.

## Ophis CLI
Quote, swap and bridge from your terminal, with every step approved in your own phone wallet (keys never leave it).
- npm: [`@ophis/cli`](https://www.npmjs.com/package/@ophis/cli), install with `npm install -g @ophis/cli` (Node.js 20 or later)
- Guide: [docs.ophis.fi/cli](https://docs.ophis.fi/cli)

## Widget
An embeddable swap widget for a brand-light integration (frame-embeddable; wallet signing stays out of frame).
- See `examples/widget-embed` in the monorepo.

## Examples
Drop-in integration examples (React/Next.js/Node/Python/iframe + AI-agent frameworks) live in the monorepo's `examples/` and in the per-framework repos under this org.

## Chains
Ethereum, Optimism, BNB Chain, Gnosis, Polygon, Base, Plasma, Arbitrum, Avalanche, Ink, Linea. Cross-chain destinations on Solana and Bitcoin via NEAR Intents.

## Earn (referral rebate)
Embed via the SDK or the MCP server with your referral code in the appData, and earn 8 to 12 percent of the net fee on every swap your users make. The referral sticks on-chain. See [docs.ophis.fi](https://docs.ophis.fi).

## Links
- App: https://ophis.fi
- Docs: https://docs.ophis.fi
- SDK: https://www.npmjs.com/package/@ophis/sdk
- CLI: https://www.npmjs.com/package/@ophis/cli
- Source: https://github.com/ophis-fi/ophis
- X: https://x.com/ophis_fi

## Contributing
Built an Ophis integration? Open a PR adding it here. Keep entries to one line: name, link, and what it does.
