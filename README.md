# apeir

Small, tested open-source tools for Neo N3, the Nym mixnet, Zcash, Stacks and Tezos, plus code reviews and fixes
for crypto projects. Everything here is MIT unless a repo says otherwise.

**Hire me:** paid tool builds, pre-deploy contract reviews and bug fixes, priced per task and paid in crypto.
Open an issue on [apeirs/apeirs](https://github.com/apeirs/apeirs/issues) with the task and your budget.
Pre-deploy Clarity reviews have a fixed price: [15,000 sats per contract](clarity-reviews.md).

## Neo N3

| Tool | What it does |
|---|---|
| [n3-trace](https://github.com/apeirs/n3-trace) | Read any transaction like a debugger (decoded calls, call tree, storage diffs) and preview one before you sign it |
| [n3-lineage](https://github.com/apeirs/n3-lineage) | Upgrade history and manifest/NEF diffs for any contract |
| [n3-snapshot](https://github.com/apeirs/n3-snapshot) | Verifiable NEP-17 / NEP-11 holder snapshots and NEO vote tallies at any block |

All three use public RPC only: no keys, no indexer, Python standard library.

## Nym mixnet integrations

Send a wallet's or tool's traffic through the Nym mixnet instead of the clear net:
[nymdial](https://github.com/apeirs/nymdial) (Rust, in-process TCP/TLS),
[nymleak](https://github.com/apeirs/nymleak) (proves a program leaks nothing around Nym),
[zecmix](https://github.com/apeirs/zecmix) ·
[xmrmix](https://github.com/apeirs/xmrmix) ·
[mixpool](https://github.com/apeirs/mixpool) (Bitcoin) ·
[ethmix](https://github.com/apeirs/ethmix) ·
[solanamix](https://github.com/apeirs/solanamix) ·
[cosmosmix](https://github.com/apeirs/cosmosmix) ·
[dotmix](https://github.com/apeirs/dotmix) ·
[stxmix](https://github.com/apeirs/stxmix) ·
[trxmix](https://github.com/apeirs/trxmix) ·
[nostrmix](https://github.com/apeirs/nostrmix) ·
[cashumix](https://github.com/apeirs/cashumix) ·
[dnsmix](https://github.com/apeirs/dnsmix) ·
[aptmix](https://github.com/apeirs/aptmix) ·
[mixdate](https://github.com/apeirs/mixdate)

## Other chains

- [stakeclock](https://github.com/apeirs/stakeclock): when unstaked tez becomes spendable (Tezos, read-only CLI)
- [xmrpool](https://github.com/apeirs/xmrpool): read the Monero tx pool from restricted public nodes
- [sparkname](https://github.com/apeirs/sparkname): move a Firo Spark Name between wallets safely
- [pot](https://github.com/apeirs/pot): a no-backend Bitcoin Cash bounty pot (CashScript)
- [tripwire](https://github.com/apeirs/tripwire): cross-chain drain guard on Reactive Network
- [gib-escrow](https://github.com/apeirs/gib-escrow): check whether a Gibwork bounty is really funded

## Merged upstream

- ShieldedLabs/crosslink_monolith: fixes for #325 (small-order finalizer keys) and #331 (wallet RPCs without a wallet)
- bisq-network/bisq-musig and bisq-network/bisq: RPC wallet-readiness and seednode install fixes
- ZecHub/zechub: wallet documentation corrections
- aibtcdev/aibtc-mcp-server: spend-cap test hardening
