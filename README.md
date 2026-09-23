# Awesome Arc [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of the **Arc** ecosystem — Circle's L1 where **USDC is the native gas token**.
Mainnet opened 2026-09-16. PRs welcome.

## Chain facts

- Chain ID: **5042** (`0x13b2`)
- Native currency: **USDC** — 18 decimals as `msg.value`; the same balance has a
  6-decimal ERC-20 view at `0x3600000000000000000000000000000000000000`
- Block time: ~510 ms
- RPC: `https://rpc.mainnet.arc.io` (public; also served via dRPC and QuickNode prefixes)
- Explorer: [explorer.arc.io](https://explorer.arc.io)
- Site: [arc.io](https://www.arc.io) · Built by [Circle](https://www.circle.com)

## Core infrastructure

- **Uniswap v4** (canonical) — PoolManager `0x8366a39CC670B4001A1121B8F6A443A643e40951`,
  PositionManager `0x6049c9a0e26405C0985f9E3685C87d0aE917f82B`,
  Universal Router `0x4fcA4a51Ab4F23A7447b3284fBd7D73289A89Fb1`,
  StateView `0xF3334192D15450CdD385c8B70e03f9A6bD9E673b`
- **Uniswap Liquidity Launcher** `0x0000FffFBE8efE702c8703aE3477FF5dE3d319C0` —
  [open-source token launch system](https://github.com/Uniswap/liquidity-launcher) (v3.2.0)
- **Permit2** `0x000000000022D473030F116dDEE9F6B43aC78BA3`

## Launchpads

- [SolonPad](https://solonpad.fun) — USDC-native launchpad; tokens are born directly in
  Uniswap v4 pools (LP locked forever) with an optional progressive bonding-curve mode.
  Launch contracts Sourcify-verified · [agent skill](https://github.com/solonlend/solonpad-skill)
  lets AI agents launch and trade without the site.
  [SOLON staking](https://solonpad.fun/stake) streams the daily platform-fee buyback to
  stakers over 7 days; no lock, no cooldown
  ([source](https://github.com/solonlend/solonpad-contracts/tree/main/src/stake)).
- [minara.fun](https://minara.fun) — launchpad built on the UERC20 factory with a custom
  fee hook; platform token Minara.
- [bozo.fun](https://bozo.fun) — launchpad; platform token BOZO.

## Data & aggregators

- [GeckoTerminal — Arc](https://www.geckoterminal.com/arc/pools) (network key `arc`)
- [DexScreener — Arc](https://dexscreener.com/arc)
- [GMGN — Arc](https://gmgn.ai/?chain=arc)
- [DefiLlama](https://defillama.com) — chain key `arc`

## Bridges & on-ramps

- [Relay](https://relay.link) — fast RH/EVM ↔ Arc transfers and same-chain swaps API
- [LI.FI](https://li.fi) — aggregated routes to Arc (choose non-intent bridges for speed)

## Agent tooling

- [solonpad-skill](https://github.com/solonlend/solonpad-skill) — machine interface for
  launching/trading on SolonPad: pinned addresses, ABIs, READ→VERIFY→USE call sequences
- [arcpay](https://github.com/Puneethkumarck/arcpay) — open-source payment protocol on Arc
  for AI-agent payments

## Contributing

Open a PR. Entries must be live on Arc mainnet (5042), with a working link; verified
sources (Sourcify/explorer) preferred.
