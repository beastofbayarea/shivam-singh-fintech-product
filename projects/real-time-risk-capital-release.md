# D. E. Shaw Real-Time Risk — Capital Release at Trading Speed

## What I worked on

I completed this work during my [D. E. Shaw experience from July 2016 to December 2019](https://github.com/beastofbayarea/shivam-singh-fintech-product/blob/main/shivam-singh-fintech-product.pdf).

I built a unified, streaming risk gate that governed each transaction at execution speed. A common trade model, deterministic capital checks, explainable fraud detection, degraded-mode controls, and a three-month shadow period replaced slow retrospective risk without rewriting proven quantitative libraries.

## At a glance

- I led a $10M real-time risk platform that reduced transaction checks from 90 ms to 4.2 ms and false positives by roughly 90%.
- I released $85M in regulatory capital and blocked $15M of harmful exposure through explainable, event-level capital and fraud controls.
- I migrated asset classes through a common trade model and three-month shadow validation, achieving approximately 98% agreement with established risk outcomes before authority transfer.

## The situation

Overnight calculations hid intraday exposure, a vendor check destroyed time-sensitive execution value, opaque fraud scores sent 15% of trades to manual review, and desk-specific data models prevented consolidated risk.

## What I needed to accomplish

I needed to move risk from retrospective reporting into the transaction path while satisfying trading speed, capital accuracy, fraud detection, auditability, and continuity requirements.

## What I did

- I normalized bonds, derivatives, and digital assets into one trade ontology.
- I kept mature quantitative libraries behind adapters while replacing the fragmented data and execution layer.
- I combined deterministic regulatory calculations with probabilistic detection and human-readable reasons.
- I mirrored live traffic for three months and retained hard exposure limits in degraded mode.

## The results

- Latency fell from 90 ms to 4.2 ms.
- False positives declined approximately 90%.
- The system blocked $15M in harmful exposure and unlocked $85M in regulatory capital.
- I risked outcomes matched the established process about 98% of the time during shadow validation.

## Decisions and trade-offs

- I used phased replacement instead of a big-bang rewrite.
- I treated explainability and the shared trade model as equal to raw latency.
- I failed into tighter risk limits rather than unrestricted bypass.

## How I led

I aligned traders, quant researchers, compliance, risk, engineers, and capital partners around a single latency, accuracy, resilience, and capital-value scorecard.

## Why I chose this approach

I used [Basel Committee - BCBS 239 (2013)](https://www.bis.org/publ/bcbs239.htm) to ground risk-data aggregation, governance, quality, and reporting principles. I used [Basel Committee - Revised market-risk framework (2016)](https://www.bis.org/press/p160114.htm) to ground contemporaneous market-risk, expected-shortfall, stress, and liquidity-horizon context.

## Sources and external context

I used independent methodology and market evidence to shape the work. The resume link above is included only to establish the employment timeline.

| Source | How it informed my work | Timing |
|---|---|---|
| [Basel Committee - BCBS 239 (2013)](https://www.bis.org/publ/bcbs239.htm) | I used it to ground risk-data aggregation, governance, quality, and reporting principles. | — |
| [Basel Committee - Revised market-risk framework (2016)](https://www.bis.org/press/p160114.htm) | I used it to ground contemporaneous market-risk, expected-shortfall, stress, and liquidity-horizon context. | — |
