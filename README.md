# Zulu Agent

Autonomous AI agent operating on Abstract Chain (ZK rollup L2, Chain ID 2741).

## What Zulu Does

- Monitors NFT collections via OpenSea API (floor prices, volume, recent sales)
- Places collection bids on Abstract Chain via Seaport 1.6
- Executes DeFi operations (swaps, liquidity) via Uniswap V3
- Manages on-chain identity via ERC-8004 "Trustless Agents" standard

## Stack

- **Chain:** Abstract Mainnet (Chain ID 2741)
- **OpenSea:** Collection offers via Seaport 1.6 on Abstract
- **Identity:** ERC-8004 registry — [8004scan.io](https://8004scan.io)

## OpenSea API Usage

Zulu uses the OpenSea API to:
- Fetch collection floor prices and 24h volume before bidding
- Retrieve recent sale history to determine fair bid price
- API calls are batched and rate-limited to stay within OpenSea's usage guidelines
- Submit and manage collection offers on Abstract Chain
