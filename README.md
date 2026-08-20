# Airdrop Farming ROI (Sample)

Sample dataset analyzing historical cryptocurrency airdrops â€” farming cost, actual payouts, ROI, and eligibility criteria across 20 major protocols.

## What's Inside

This sample contains **20 airdrop events** from 2020-2026 across Ethereum, Base, Arbitrum, Optimism, Solana, and Cosmos:

| Column | Type | Description |
|--------|------|-------------|
| protocol | string | Protocol that conducted the airdrop |
| token_symbol | string | Ticker of the dropped token |
| airdrop_date | ISO date | When tokens were claimable |
| total_tokens_dropped | int | Total tokens distributed |
| total_value_usd | int | Total value at TGE price |
| farmers_count | int | Estimated number of recipients |
| avg_farming_duration_days | int | Average time spent farming before airdrop |
| est_farming_cost_usd | int | Estimated gas/fees spent to qualify |
| avg_payout_per_farmer_usd | int | Average USD value received per farmer |
| median_payout_usd | int | Median payout (more representative than mean) |
| roi_pct | int | Return on investment: (payout - cost) / cost Ã— 100 |
| eligibility_criteria | string | What users had to do to qualify |
| farming_complexity | string | low / medium / high effort required |
| chain | string | Primary chain of the protocol |

## Key Observations

| Metric | Value |
|--------|-------|
| Best ROI | Hyperliquid â€” 19,688% (avg cost $50, avg payout $9,894) |
| Worst ROI | Base (speculative) â€” -100% ($500 spent, $0 received, no airdrop yet) |
| Highest payout | Ethena â€” $7,105 avg per farmer |
| Lowest payout | Linea â€” $952 avg, but median only $85 |
| No-cost wins | Uniswap, Optimism, Arbitrum, Jito â€” retroactive, zero farming cost |
| Most farmers | Starknet â€” 1.29M recipients |

**Patterns:**
- **Retroactive airdrops** (Uniswap, Arbitrum, Optimism) had highest payouts with zero cost
- **Continuous farming** (Base speculation, Linea) often results in negative ROI due to gas costs
- **Complex criteria** (Linea, Puffer, Starknet) don't always correlate with higher payouts
- **Trading volume-based** (Hyperliquid, Ethena) tends to reward whales disproportionately

## Use Cases

- Airdrop farming strategy optimization
- Protocol token launch research
- Cost-benefit analysis for farming campaigns
- Academic research on token distribution mechanisms
- Building airdrop prediction models

## Full Dataset

The complete dataset covers **80+ airdrop events** with detailed eligibility criteria breakdowns, snapshot dates, vesting schedules, and post-TGE price performance.

- **Payhip:** [Manteclaw Datasets](https://payhip.com/Manteclaw)
- **Full rows:** 80+
- **Price:** $14

## Methodology

Airdrop data collected from official announcements, on-chain claim contracts, and Dune Analytics dashboards. Farming cost estimated from average gas spent per qualifying action Ã— actions required. Payout calculated at Token Generation Event price (not peak). ROI = (median_payout - farming_cost) / farming_cost.

## License

CC BY 4.0 â€” Attribution required. Commercial use permitted.

---
*Sample dataset for evaluation. Full version available on Payhip.*
