---
name: junct-defi
description: Access 19 live DeFi protocol MCP servers via Junct. Real-time data for Aave, Chainlink, Pyth, GMX, CoinGecko, DeFiLlama, Curve, Binance, EigenLayer, Lido, Synthetix, Maker, ENS, Euler, Stargate, Blockscout, Beefy, Jupiter and Compound. Free. No auth. No API key. Deterministic generation.
tags: defi, crypto, mcp, price, tvl, yield, oracle, dex, lending, staking, bridge, analytics, agent-ready, web3, ethereum, solana, binance
---

# Junct DeFi — 19 Live Protocol MCP Servers

Junct is the agent-readiness layer for the crypto stack. All servers are deterministically generated from official API specs — 1:1 endpoint-to-tool coverage, no AI generation, fully auditable.

Every server below is live, free, and requires no API key. Connect via MCP (Streamable HTTP transport) from Claude Desktop, Cursor, Windsurf, OpenClaw, or any MCP-compatible agent.

## Server Directory

### Prices & Oracles

- **Pyth** — Sub-second price feeds for 500+ assets
  `https://pyth-hermes.mcp.junct.dev/mcp`
  Key tools: get_latest_price_updates, get_price_feed_ids, get_twaps

- **Chainlink** — Decentralised oracle network, $20B+ secured
  `https://chainlink.mcp.junct.dev/mcp`
  Key tools: get_price_feed, get_proof, get_automation_registry

### Market Data & Analytics

- **CoinGecko** — Prices, market cap, volume for 10,000+ tokens
  `https://coingecko.mcp.junct.dev/mcp`
  Key tools: get_simple_price, get_coins_markets, get_search_trending

- **DeFiLlama** — TVL, yields, stablecoins across 200+ chains
  `https://defillama.mcp.junct.dev/mcp`
  Key tools: get_protocols, get_tvl, get_yields_pools, get_stablecoins

- **Blockscout** — On-chain explorer analytics
  `https://blockscout.mcp.junct.dev/mcp`

### Trading & DEX

- **Binance** — CEX market data, 340 tools
  `https://binance.mcp.junct.dev/mcp`

- **GMX** — Decentralised perpetuals and spot trading
  `https://gmx.mcp.junct.dev/mcp`

- **Jupiter** — Solana DEX aggregator
  `https://jupiter.mcp.junct.dev/mcp`

- **Curve** — Stablecoin AMM analytics
  `https://curve.mcp.junct.dev/mcp`

- **Synthetix** — Derivatives protocol data
  `https://synthetix.mcp.junct.dev/mcp`

### Lending & Vaults

- **Aave** — Largest lending protocol, rates and positions
  `https://aave.mcp.junct.dev/mcp`

- **Maker** — DAI and Sky protocol data
  `https://maker.mcp.junct.dev/mcp`

- **Euler** — Modular lending markets
  `https://euler.mcp.junct.dev/mcp`

- **Compound** — Lending and borrowing rates
  `https://compound.mcp.junct.dev/mcp`

- **Beefy** — Yield vault analytics
  `https://beefy.mcp.junct.dev/mcp`

### Staking & Liquid Staking

- **Lido** — Largest liquid staking protocol
  `https://lido.mcp.junct.dev/mcp`

- **EigenLayer** — Restaking protocol analytics
  `https://eigenlayer.mcp.junct.dev/mcp`

### Infrastructure

- **Stargate** — Cross-chain bridge data
  `https://stargate.mcp.junct.dev/mcp`

- **ENS** — Ethereum Name Service lookups
  `https://ens.mcp.junct.dev/mcp`

## How to Connect

All servers use Streamable HTTP transport. Add to your MCP client config:

```json
{
  "mcpServers": {
    "pyth": {
      "url": "https://pyth-hermes.mcp.junct.dev/mcp",
      "transport": "streamable-http"
    },
    "defillama": {
      "url": "https://defillama.mcp.junct.dev/mcp",
      "transport": "streamable-http"
    },
    "coingecko": {
      "url": "https://coingecko.mcp.junct.dev/mcp",
      "transport": "streamable-http"
    }
  }
}
```

## Example Queries

- "What's the current price of ETH?" → Pyth or CoinGecko
- "Show me the top 10 DeFi protocols by TVL" → DeFiLlama
- "What are the current Aave lending rates for USDC?" → Aave
- "Get the latest Binance BTC/USDT order book" → Binance
- "What's the stETH/ETH exchange rate on Lido?" → Lido
- "Show me active EigenLayer operators" → EigenLayer
- "Resolve vitalik.eth" → ENS

## Discovery

- All servers: https://junct.dev/servers
- Full tool list: https://junct.dev/llms-full.txt
- One-click configs: https://junct.dev/servers/{protocol}
- llms.txt directory: https://api.junct.dev/llms.txt
