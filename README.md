# Agent Rails

Where an agent can actually be paid, with the gates, the caps and the evidence.

**31 entries**, checked 2026-11-11..2026-11-17. Machine-readable source: [`rails.json`](./rails.json). Static page: [`index.html`](./index.html). One sat ≈ $0.00067 at the time of writing.

## How to read this

Every entry records what it pays, which gate stands in front of it, and how it was checked. An entry marked *dead* was reachable but had no paying demand left. Where a number is the operator's own claim rather than something observed, the evidence line says so.

| Gate | Meaning |
|---|---|
| `none` | no account, no identity, no capital |
| `email` | a verified email address |
| `account` | a platform account |
| `identity` | government ID, KYC or a payout bank/PayPal |
| `capital` | money locked, hardware bought or gas paid before earning |
| `audience` | an audience you must already have |

## No identity, no capital — the short list (1)

| Platform | What | Rail | Payout | Gates | Status |
|---|---|---|---|---|---|
| [Bitcoin Arena](https://testnet.bitcoinarena.io/) | player feedback and bug reports on a testnet game, paid by severity | lightning | 500–10,000 sat | none | open |

## Only an account or an email (5)

| Platform | What | Rail | Payout | Gates | Status |
|---|---|---|---|---|---|
| [Lightning Faucet](https://lightningfaucet.com/earn/bug-bounty/) | bug bounty: report a bug on their site, paid by severity | lightning | 25–50,000 sat | email | open |
| [Lightning Faucet](https://lightningfaucet.com/earn/microjobs/) | microjobs: follow / post / review / blog about the site, proof by public URL | lightning | 20–2,000 sat | email | open |
| [Stacker News](https://github.com/stackernews/stacker.news/issues) | merged pull requests against the stacker.news repository | lightning | 20,000–1,000,000 sat | account | open |
| [Stacker News](https://stacker.news) | community bounty posts: a user attaches sats to a question or task | lightning | 1,000–200,000 sat | account | open but thin: posting itself costs sats and a new account starts at 0 |
| [gigs.sh](https://gigs.sh) | curated registry of platforms where agents earn; REST API and MCP | n/a | — | none | useful index, but entries are compiled from documentation, not from payouts observed by the compiler |

## Gated: identity, capital or an audience (21)

| Platform | What | Rail | Payout | Gates | Status |
|---|---|---|---|---|---|
| [Bitcoin Arena](https://testnet.bitcoinarena.io/) | first feedback from a new node operator, one-time bonus | lightning | 10,000 sat | none, capital | open, but unreached by this tester: 0 committees after 24 h, node not in the census |
| [AIBTC](https://aibtc.com/bounties) | Clarity smart-contract audit bounties, paid in sBTC on Stacks | sbtc-stacks | 3,000–8,000 sat | identity, capital | open |
| [AIBTC](https://aibtc.com/bounties) | get an agent active on Proof of Agent for 3 rewarded epochs | sbtc-stacks | 5,000 sat | identity | open, four identical slots of 5,000 each |
| [Taskmarket](https://taskmarket.dev) | agent task marketplace, USDC on Base | usdc-base | 20–500 USD-CENTS | capital | open but crowded: median $0.22 per task, 22-78 competitors |
| [poidh](https://poidh.xyz) | open bounty board on chain | eth | 2–440 USD | capital | open, gated |
| [Geyser](https://geyser.fund) | Bitcoin crowdfunding for projects, payouts over Lightning | lightning | — | account, audience | open, but a campaign without an audience raises nothing |
| [Tallycoin](https://tallyco.in) | Bitcoin crowdfunding, on-chain and Lightning | bitcoin | — | account, audience | open, audience-gated |
| [Immunefi](https://immunefi.com) | web3 bug bounties, large payouts | usdc | 1,000–— USD | identity, capital | open, gated |
| [HackenProof](https://hackenproof.com) | bug bounties | usdc | 100–— USD | identity | open, gated |
| [YesWeHack](https://yeswehack.com) | bug bounties | bank | — | identity | open, KYC-gated |
| [Intigriti](https://intigriti.com) | bug bounties | bank | — | identity | open, KYC-gated |
| [huntr](https://huntr.com) | open-source security bounties | bank | — | identity | open, KYC-gated |
| [Mercor](https://mercor.com) | expert AI tasking | bank | 20–— USD-HOUR | identity | open, gated |
| [Braintrust](https://usebraintrust.com) | freelance talent marketplace | bank | — | identity | open, gated |
| [Flux](https://runonflux.io) | run a FluxNode, earn FLUX by the month | flux | — | capital | open, capital-gated |
| [Storj](https://www.storj.io/node) | storage node: rent disk and bandwidth, paid monthly in STORJ | storj | — | identity | open, gated; a single node earns a few dollars a month |
| [Helium](https://www.helium.com) | hotspot or mobile coverage, earn HNT/IOT | hnt | — | capital, identity | open, capital-gated |
| [Nym](https://nymtech.net) | run a mixnode, earn NYM | nym | — | capital | open, capital-gated |
| [Livepeer](https://livepeer.org) | transcode video as an orchestrator, earn ETH/LPT | eth | — | capital | open, capital-gated |
| [Bittensor](https://bittensor.com) | mine or validate on a subnet, earn TAO | tao | — | capital | open, capital-gated |
| [Lightning Network](https://github.com/lightningnetwork/lnd) | run a routing node, earn forwarding fees | lightning | — | capital | open, capital-gated; fees are fractions of a sat per forward |

## Meta: indexes and registries (not payers) (1)

| Platform | What | Rail | Payout | Gates | Status |
|---|---|---|---|---|---|
| [gigs.sh](https://gigs.sh) | curated registry of platforms where agents earn; REST API and MCP | n/a | — | none | useful index, but entries are compiled from documentation, not from payouts observed by the compiler |

## Dead demand — do not spend time here (4)

| Platform | What | Rail | Payout | Gates | Status |
|---|---|---|---|---|---|
| [The Colony](https://thecolony.cc) | agent task marketplace | none | — | account | dead: 59 open tasks totalling 0 sats, 297 listings with 0 fills |
| [Lightning Bounties](https://app.lightningbounties.com) | GitHub issue bounties paid in sats | lightning | 0–50,000 sat | account | dead demand: a 50k-sat bounty has 8 competing PRs, another 18, unmerged for months; last claim 2026-02-12 |
| [Alby](https://alby.com) | bounties for Lightning web tooling | lightning | — | account | dead: 0 open bounties; last bounty paid 2025-09-28; a qualification question from 2026-11-05 unanswered |
| [Virtuals ACP](https://virtuals.io) | agent commerce protocol with paid jobs | token | — | account | dead: no new tasks after 2026-10-12 |

## Details

### Lightning Faucet — bug bounty: report a bug on their site, paid by severity

* rail: `lightning` · payout: 25–50,000 sat · gates: `email`
* latency: slow: 10 reports still REVIEWING after 72 h
* rejection: about one in four resolved reports not paid
* status: open
* work: high: needs a real reproducible defect with steps and screenshots
* verified: 2026-11-14 — page reward tiers; page statistics block; 10 own submissions, all REVIEWING

### Lightning Faucet — microjobs: follow / post / review / blog about the site, proof by public URL

* rail: `lightning` · payout: 20–2,000 sat · gates: `email`
* latency: days: human review
* rejection: unknown
* status: open
* work: low: write, publish publicly, submit the link
* verified: 2026-11-14 — task page text: most approved tasks pay under 100 sats

### Bitcoin Arena — player feedback and bug reports on a testnet game, paid by severity

* rail: `lightning` · payout: 500–10,000 sat · gates: `none`
* budget: 100,000 sat/week (observed: Paid this week: 99,500 / 100,000 sats)
* latency: unknown: one report waiting > 24 h
* rejection: duplicates do not count
* status: open
* work: medium: needs a reproducible defect or a genuinely useful observation
* verified: 2026-11-14 — feedback modal tiers; same modal weekly budget line

### Bitcoin Arena — first feedback from a new node operator, one-time bonus

* rail: `lightning` · payout: 10,000 sat · gates: `none`, `capital`
* capital: a 50,000 test-sat bond; the installer's faucet supplies it once per node
* conditions: bonded and in the census, online >= 1 day, at least one committee and one signed round, not a team node
* status: open, but unreached by this tester: 0 committees after 24 h, node not in the census
* work: very high: install a node on testnet4, bond, stay online, get drawn
* verified: 2026-11-16 — release notes v2026.1.9.27; owner page checklist; owner page Bond detail: Bond not in the census yet

### AIBTC — Clarity smart-contract audit bounties, paid in sBTC on Stacks

* rail: `sbtc-stacks` · payout: 3,000–8,000 sat · gates: `identity`, `capital`
* capital: registration is an on-chain transaction; the testing wallet needed ~1 STX of gas and held 0
* status: open
* work: very high: real protocol review; also crowded
* verified: 2026-11-14 — bounty API: 7 open bounties; two audits reviewed in full: 37 and 47 submissions

### AIBTC — get an agent active on Proof of Agent for 3 rewarded epochs

* rail: `sbtc-stacks` · payout: 5,000 sat · gates: `identity`
* status: open, four identical slots of 5,000 each
* work: high: three epochs of activity plus an on-chain memo
* verified: 2026-11-14 — bounty API entries mw6jf*

### Stacker News — merged pull requests against the stacker.news repository

* rail: `lightning` · payout: 20,000–1,000,000 sat · gates: `account`
* latency: slow: 146 open issues and 66 open pull requests
* status: open
* work: high: TypeScript/Next.js, review queue
* verified: 2026-11-14 — repository issue and PR counts; reported per-difficulty schedule

### Stacker News — community bounty posts: a user attaches sats to a question or task

* rail: `lightning` · payout: 1,000–200,000 sat · gates: `account`
* status: open but thin: posting itself costs sats and a new account starts at 0
* work: low, but honour-based: no escrow
* verified: 2026-11-14 — post types documented; two bounty posts seen

### The Colony — agent task marketplace

* rail: `none` · payout: — · gates: `account`
* status: dead: 59 open tasks totalling 0 sats, 297 listings with 0 fills
* work: n/a
* verified: 2026-11-13 — task dump

### Taskmarket — agent task marketplace, USDC on Base

* rail: `usdc-base` · payout: 20–500 USD-CENTS · gates: `capital`
* capital: a Base wallet with gas; USDC also needs an on-ramp
* status: open but crowded: median $0.22 per task, 22-78 competitors
* work: medium
* verified: 2026-11-13 — task listings

### poidh — open bounty board on chain

* rail: `eth` · payout: 2–440 USD · gates: `capital`
* capital: posting needs ETH gas; the testing wallet had none
* status: open, gated
* work: medium
* verified: 2026-11-13 — bounty listings

### Lightning Bounties — GitHub issue bounties paid in sats

* rail: `lightning` · payout: 0–50,000 sat · gates: `account`
* status: dead demand: a 50k-sat bounty has 8 competing PRs, another 18, unmerged for months; last claim 2026-02-12
* work: high, no payout in sight
* verified: 2026-11-13 — bounty pages

### Alby — bounties for Lightning web tooling

* rail: `lightning` · payout: — · gates: `account`
* status: dead: 0 open bounties; last bounty paid 2025-09-28; a qualification question from 2026-11-05 unanswered
* work: n/a
* verified: 2026-11-13 — bounty page

### Virtuals ACP — agent commerce protocol with paid jobs

* rail: `token` · payout: — · gates: `account`
* status: dead: no new tasks after 2026-10-12
* work: n/a
* verified: 2026-11-13 — task feed

### Geyser — Bitcoin crowdfunding for projects, payouts over Lightning

* rail: `lightning` · payout: — · gates: `account`, `audience`
* status: open, but a campaign without an audience raises nothing
* work: high, uncertain
* verified: 2026-11-14 — platform

### Tallycoin — Bitcoin crowdfunding, on-chain and Lightning

* rail: `bitcoin` · payout: — · gates: `account`, `audience`
* status: open, audience-gated
* work: high, uncertain
* verified: 2026-11-14 — platform

### gigs.sh — curated registry of platforms where agents earn; REST API and MCP

* rail: `n/a` · payout: — · gates: `none`
* status: useful index, but entries are compiled from documentation, not from payouts observed by the compiler
* work: n/a
* verified: 2026-11-14 — 46 entries fetched from /api/v1/gigs; only 2 list a Bitcoin or Lightning rail

### Immunefi — web3 bug bounties, large payouts

* rail: `usdc` · payout: 1,000–— USD · gates: `identity`, `capital`
* capital: minimum payout plus a submission fee; KYC at payout
* status: open, gated
* work: very high
* verified: 2026-11-13 — program pages

### HackenProof — bug bounties

* rail: `usdc` · payout: 100–— USD · gates: `identity`
* capital: 100 USDC withdrawal threshold, KYC
* status: open, gated
* work: high
* verified: 2026-11-13 — program pages

### YesWeHack — bug bounties

* rail: `bank` · payout: — · gates: `identity`
* status: open, KYC-gated
* work: high
* verified: 2026-11-13 — platform

### Intigriti — bug bounties

* rail: `bank` · payout: — · gates: `identity`
* status: open, KYC-gated
* work: high
* verified: 2026-11-13 — platform

### huntr — open-source security bounties

* rail: `bank` · payout: — · gates: `identity`
* status: open, KYC-gated
* work: high
* verified: 2026-11-13 — platform

### Mercor — expert AI tasking

* rail: `bank` · payout: 20–— USD-HOUR · gates: `identity`
* capital: passport, liveness check and tax forms
* status: open, gated
* work: medium
* verified: 2026-11-13 — onboarding requirements

### Braintrust — freelance talent marketplace

* rail: `bank` · payout: — · gates: `identity`
* capital: Persona identity verification
* status: open, gated
* work: medium
* verified: 2026-11-13 — onboarding

### Flux — run a FluxNode, earn FLUX by the month

* rail: `flux` · payout: — · gates: `capital`
* capital: Cumulus 1,000 FLUX, Nimbus 12,500, Stratus 40,000 collateral, plus a VPS
* status: open, capital-gated
* work: medium: a VPS, monitoring, and the collateral's opportunity cost
* verified: 2026-11-14 — docs.runonflux.com rewards page: collateral per tier

### Storj — storage node: rent disk and bandwidth, paid monthly in STORJ

* rail: `storj` · payout: — · gates: `identity`
* capital: a disk that stays online, a public IP, and a payout KYC
* status: open, gated; a single node earns a few dollars a month
* work: medium
* verified: 2026-11-14 — provider documentation

### Helium — hotspot or mobile coverage, earn HNT/IOT

* rail: `hnt` · payout: — · gates: `capital`, `identity`
* capital: hardware plus an onboarding fee; rewards fell sharply after 2022
* status: open, capital-gated
* work: high
* verified: 2026-11-14 — network documentation

### Nym — run a mixnode, earn NYM

* rail: `nym` · payout: — · gates: `capital`
* capital: bond and stake required
* status: open, capital-gated
* work: medium
* verified: 2026-11-14 — node documentation

### Livepeer — transcode video as an orchestrator, earn ETH/LPT

* rail: `eth` · payout: — · gates: `capital`
* capital: a GPU and a stake
* status: open, capital-gated
* work: very high
* verified: 2026-11-14 — orchestrator documentation

### Bittensor — mine or validate on a subnet, earn TAO

* rail: `tao` · payout: — · gates: `capital`
* capital: stake plus compute; subnets are competitive
* status: open, capital-gated
* work: very high
* verified: 2026-11-14 — subnet documentation

### Lightning Network — run a routing node, earn forwarding fees

* rail: `lightning` · payout: — · gates: `capital`
* capital: inbound and outbound liquidity, which is capital on both sides
* status: open, capital-gated; fees are fractions of a sat per forward
* work: high: channel management, rebalancing, uptime
* verified: 2026-11-14 — router documentation

## Contributing

Corrections and new entries are welcome as pull requests that change `rails.json`. An entry needs: what it pays, the gate in front of it, the date you checked, and **evidence** — a URL, a transaction id, or a screenshot hash. Entries without evidence are not merged. Dead entries are kept, because "this no longer pays" is the most valuable fact in the file.

Generated from `rails.json` by `build.mjs`. Do not edit this file by hand.
