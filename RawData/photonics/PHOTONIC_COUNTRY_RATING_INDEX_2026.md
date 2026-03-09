# Photonic Quantum Country Rating Index (PQCRI-2026)

Date: 2026-03-07
Purpose: A reusable index to score and compare countries on photonic quantum computing readiness and execution.

## How scoring works

Each country is scored 1-5 on 6 dimensions, then weighted.

Dimensions:
- `Policy & Funding` (weight 25%): national strategy clarity, budget continuity, mission execution.
- `Research Depth` (weight 20%): university/lab quality, talent pipeline, publication strength.
- `Industry Strength` (weight 20%): active photonic-quantum companies, scale-ups, corporate partnerships.
- `Deployment & Infrastructure` (weight 15%): public testbeds, on-prem systems, manufacturing/pilot assets.
- `Global Integration` (weight 10%): cross-border collaboration and ecosystem influence.
- `Commercial Momentum` (weight 10%): customer pilots, contracts, translation from R&D to market.

Formula:
`Weighted Score (0-100) = ((Policy*0.25 + Research*0.20 + Industry*0.20 + Deployment*0.15 + Global*0.10 + Commercial*0.10) / 5) * 100`

## Rating bands

- `85-100`: Global Leader
- `70-84`: Strong Contender
- `55-69`: Emerging Power
- `40-54`: Developing Ecosystem
- `<40`: Early Stage

## Country scorecard (current pack)

| Country | Policy | Research | Industry | Deployment | Global | Commercial | Weighted Score | Rating |
|---|---:|---:|---:|---:|---:|---:|---:|---|
| United States | 5 | 5 | 5 | 4 | 5 | 5 | 96 | Global Leader |
| United Kingdom | 5 | 5 | 4 | 4 | 5 | 4 | 89 | Global Leader |
| Canada | 5 | 5 | 5 | 4 | 4 | 4 | 91 | Global Leader |
| China | 5 | 5 | 4 | 4 | 3 | 4 | 85 | Global Leader |
| Netherlands | 4 | 5 | 4 | 4 | 4 | 4 | 82 | Strong Contender |
| Japan | 4 | 5 | 4 | 3 | 4 | 3 | 77 | Strong Contender |
| Australia | 5 | 4 | 3 | 4 | 3 | 3 | 76 | Strong Contender |
| Singapore | 5 | 4 | 3 | 3 | 4 | 3 | 75 | Strong Contender |
| France | 4 | 4 | 4 | 3 | 4 | 3 | 75 | Strong Contender |
| South Korea | 4 | 4 | 3 | 3 | 4 | 3 | 71 | Strong Contender |
| Germany | 4 | 4 | 3 | 3 | 4 | 3 | 71 | Strong Contender |
| Israel | 3 | 4 | 3 | 2 | 4 | 3 | 62 | Emerging Power |

## Notes

- This index is designed for comparative tracking, not absolute scientific ranking.
- Scores should be reviewed quarterly as new funding, deployments, and company milestones are announced.
- If you want a stricter investor lens, increase `Commercial Momentum` to 20% and reduce `Research Depth` to 10%.
