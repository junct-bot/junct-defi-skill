---
name: junct-defi
description: Access 28 live crypto protocol MCP servers via Junct — exchanges, oracles, analytics, lending, staking, DEXes, derivatives, bridges and naming. Binance, Chainlink, Pyth, CoinGecko, CoinMarketCap, Uniswap, Aave, GMX, Lido, ENS and more. Free. No auth. Deterministic generation.
tags: defi, crypto, mcp, price, tvl, yield, oracle, dex, lending, staking, bridge, analytics, agent-ready, web3, ethereum, solana, binance, crypto data, web3 data, blockchain analytics, exchange data, cross-chain, liquid staking, on-chain data, token prices, crypto market data, derivatives, perpetuals, uniswap, coinmarketcap
---

# Junct DeFi — 28 Live Protocol MCP Servers

Junct is the agent-readiness layer for the crypto stack. All servers are deterministically generated from official API specs — 1:1 endpoint-to-tool coverage, no AI generation, fully auditable.

Every server below is live, free, and requires no API key. Connect via MCP (Streamable HTTP transport) from Claude Desktop, Cursor, Windsurf, OpenClaw, or any MCP-compatible agent.

## Server Directory

### Prices & Oracles

- **Pyth** — Sub-second price feeds for 500+ assets (11 tools)
  `https://pyth-hermes.mcp.junct.dev/mcp`

- **Chainlink** — Feed Registry — query any price feed via base/quote addresses (35 tools)
  `https://chainlink.mcp.junct.dev/mcp`

### Market Data & Analytics

- **CoinMarketCap** — Crypto market data, rankings, metadata (30 tools)
  `https://coinmarketcap.mcp.junct.dev/mcp`

- **CoinGecko** — Prices, market cap, volume for 10,000+ tokens (36 tools)
  `https://coingecko.mcp.junct.dev/mcp`

- **DeFiLlama** — TVL, yields, stablecoins across 200+ chains (59 tools)
  `https://defillama.mcp.junct.dev/mcp`

- **Etherscan** — On-chain data, balances, transactions, contracts (71 tools)
  `https://etherscan-api.mcp.junct.dev/mcp`

- **Blockscout** — On-chain explorer analytics (56 tools)
  `https://blockscout.mcp.junct.dev/mcp`

- **Coinbase** — Exchange data and market analytics (45 tools)
  `https://coinbase.mcp.junct.dev/mcp`

### Trading & DEX

- **Binance** — CEX market data (340 tools)
  `https://binance.mcp.junct.dev/mcp`

- **Uniswap** — V3 DEX, swaps and liquidity (17 tools)
  `https://uniswap.mcp.junct.dev/mcp`

- **GMX** — Decentralised perpetuals and spot trading (139 tools)
  `https://gmx.mcp.junct.dev/mcp`

- **Jupiter** — Solana DEX aggregator (4 tools)
  `https://jupiter.mcp.junct.dev/mcp`

- **Curve** — Stablecoin AMM analytics (43 tools)
  `https://curve.mcp.junct.dev/mcp`

- **ParaSwap** — Multi-chain DEX aggregator (4 tools)
  `https://paraswap.mcp.junct.dev/mcp`

- **Pendle** — Yield trading protocol (34 tools)
  `https://pendle.mcp.junct.dev/mcp`

### Derivatives

- **Synthetix** — Derivatives protocol data (22 tools)
  `https://synthetix.mcp.junct.dev/mcp`

- **Hyperliquid** — Perpetuals DEX (2 tools)
  `https://hyperliquid.mcp.junct.dev/mcp`

### Lending & Vaults

- **Aave** — Largest lending protocol (6 tools)
  `https://aave.mcp.junct.dev/mcp`

- **Maker** — DAI and Sky protocol data (10 tools)
  `https://maker.mcp.junct.dev/mcp`

- **Euler** — Modular lending markets (16 tools)
  `https://euler.mcp.junct.dev/mcp`

- **Compound** — Lending and borrowing rates (8 tools)
  `https://compound.mcp.junct.dev/mcp`

- **Beefy** — Yield vault analytics (10 tools)
  `https://beefy.mcp.junct.dev/mcp`

### Staking & Liquid Staking

- **Lido** — Largest liquid staking protocol (6 tools)
  `https://lido.mcp.junct.dev/mcp`

- **EigenLayer** — Restaking protocol analytics (8 tools)
  `https://eigenlayer.mcp.junct.dev/mcp`

### Infrastructure & Cross-Chain

- **Stargate** — Cross-chain bridge data (42 tools)
  `https://stargate.mcp.junct.dev/mcp`

- **Wormhole** — Cross-chain messaging and bridging (69 tools)
  `https://wormhole.mcp.junct.dev/mcp`

- **ENS** — Ethereum Name Service lookups (23 tools)
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
    "binance": {
      "url": "https://binance.mcp.junct.dev/mcp",
      "transport": "streamable-http"
    }
  }
}
```

## Example Queries

- "What's the current price of ETH?" — Pyth, CoinGecko, or CoinMarketCap
- "Show me the top 10 DeFi protocols by TVL" — DeFiLlama
- "What are the current Aave lending rates for USDC?" — Aave
- "Get the latest Binance BTC/USDT order book" — Binance
- "Swap 1 ETH for USDC on Uniswap" — Uniswap
- "What's the stETH/ETH exchange rate on Lido?" — Lido
- "Show me active EigenLayer operators" — EigenLayer
- "Resolve vitalik.eth" — ENS
- "Get Chainlink ETH/USD price" — Chainlink Feed Registry
- "What's the Wormhole transfer status?" — Wormhole

## Discovery

- All servers: https://junct.dev/servers
- Full tool list: https://api.junct.dev/llms-full.txt
- One-click configs: https://junct.dev/servers/{protocol}
- llms.txt directory: https://api.junct.dev/llms.txt
