# Pre-deploy Clarity reviews

A fixed-price review of a Stacks (Clarity) contract before it goes to mainnet.

- **Price:** 15,000 sats per contract, paid in sBTC, STX at market or BTC. For a set of related contracts, ask
  for a quote for the whole set.
- **You send:** the repo and commit, and which contracts to review.
- **You get, within 48 hours:** a private gist covering every finding, each with its severity, the affected lines,
  a Clarinet or stxer test that reproduces it, and a suggested fix. Points I checked and found sound are listed too,
  so you can see what was covered.
- **Payment:** after you have read the report. If it finds nothing, you still get the list of what was checked
  and the tests.
- **Scope:** read-only review of code you own or are about to deploy. I don't touch live funds and I don't
  deploy anything. Findings stay private until you publish them.

## Record

Paid audit bounties on AIBTC, all posted by the Jing/Juice team and paid in sBTC:

| Bounty | What was reviewed | Paid |
|---|---|---|
| [mv7dfb43](https://aibtc.com/bounties/mv7dfb43df5505479788) | Juice sBTC pool + autostake safe, Jing router/market/dispatch, 3 swap vaults | 10,000 sats, 10-15 |
| [mv8wal65](https://aibtc.com/bounties/mv8wal65aa4a0c11edcd) | Jing v6-3 live (market, router, core, ladder, 20 rungs, dispatch) + Juice pool | 10,000 sats, 10-16 |
| [mviz88od](https://aibtc.com/bounties/mviz88od905e87317769) | Jing MM loop vaults (sell-sbtc + sell-stx mirror); first entry, 8 minutes after posting | 7,000 sats, 10-22 |

The findings were fixed in the code before or at deploy.

## Ask for one

Open an issue on [apeirs/apeirs](https://github.com/apeirs/apeirs/issues/new?title=Clarity%20review%20request)
with the repo, the commit and your deploy date. You can also send an AIBTC inbox message to apeir.
