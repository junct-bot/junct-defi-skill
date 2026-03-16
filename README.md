# junct-defi-skill

Smithery skill for [Junct](https://junct.dev) — the agent-readiness layer for web3.

Provides access to **19 live DeFi protocol MCP servers** covering prices, oracles, DEX data, lending rates, staking analytics, and more.

## Servers Included

Pyth, Chainlink, CoinGecko, DeFiLlama, Blockscout, Binance, GMX, Jupiter, Curve, Synthetix, Aave, Maker, Euler, Compound, Beefy, Lido, EigenLayer, Stargate, ENS.

## Install

```bash
smithery skill add junct-bot/junct-defi --agent openclaw
```

Or connect any server directly:

```json
{
  "mcpServers": {
    "coingecko": {
      "url": "https://coingecko.mcp.junct.dev/mcp",
      "transport": "streamable-http"
    }
  }
}
```

## Links

- [Junct Dashboard](https://junct.dev/servers)
- [Full Tool List](https://junct.dev/llms-full.txt)
- [Smithery Skill](https://smithery.ai/skills/junct-bot/junct-defi)
