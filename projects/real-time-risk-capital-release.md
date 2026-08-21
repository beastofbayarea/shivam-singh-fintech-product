# Moving Risk Decisions into the Trading Path

I led this $10 million platform work during my [D. E. Shaw experience from July 2016 to December 2019](https://github.com/beastofbayarea/shivam-singh-fintech-product/blob/main/shivam-singh-fintech-product.pdf).

The existing process calculated important exposures overnight. A vendor check added 90 milliseconds to time-sensitive transactions, opaque fraud scores sent 15% of trades to manual review, and each desk described instruments differently. The firm could report risk after the fact, but it could not apply one reliable capital and fraud decision at execution speed.

I built the product around a demanding principle: faster risk had to be more explainable and resilient, not merely less restrictive.

## A common trade model came first

I normalized bonds, derivatives, and digital assets into one ontology for instruments, positions, counterparties, and events. This did not replace mature quantitative libraries. I kept those libraries behind adapters and replaced the fragmented data and execution layer around them.

BCBS 239 provided the primary governance frame. Its emphasis on accurate, complete, timely, and adaptable risk data reinforced why a shared model was not just an architecture preference—it was a condition for consolidated, decision-grade exposure.

## I split rules from judgment

Deterministic regulatory capital calculations remained explicit. Probabilistic fraud detection added pattern recognition, but it also produced human-readable reasons and an escalation path. That separation allowed auditors and risk owners to see which decisions came from a rule, which came from a model, and which required a person.

The Basel Committee's 2016 market-risk framework supplied contemporaneous context for expected shortfall, stress, and liquidity horizons. I translated those concepts into transaction-level gates and portfolio evidence rather than leaving them only in retrospective reports.

## Three months of shadow traffic earned authority

I mirrored live transactions through the new platform for three months while the established process remained authoritative. The comparison covered latency, capital calculations, fraud outcomes, exposure limits, availability, and audit evidence.

Asset classes moved one at a time. The new path had to reach approximately 98% agreement with established risk outcomes, explain material differences, and pass resilience tests before receiving decision authority.

I also designed the degraded mode to fail tighter. If a probabilistic service or dependency became unavailable, hard exposure limits remained active. A failure could reduce trading flexibility; it could not silently turn into unrestricted bypass.

## The economic result came from better precision

- Transaction checks fell from 90 milliseconds to 4.2 milliseconds.
- False positives declined by roughly 90%.
- The controls blocked $15 million in harmful exposure.
- More precise, current risk evidence released $85 million in regulatory capital.
- Shadow outcomes agreed with the established process about 98% of the time before transfer of authority.

The capital release was not achieved by loosening risk. It came from a more timely and granular view of the exposure that was actually present.

## How I kept the teams aligned

Traders, quant researchers, risk, compliance, engineering, and capital partners worked from one scorecard covering latency, accuracy, false positives, resilience, exposure blocked, and capital value. A speed improvement could not pass if it weakened control evidence, and a conservative model could not pass simply by blocking more trades.

## My lasting product rule

When a control enters a real-time customer or trading path, explainability and failure behavior are product requirements. I design for the moment the model disagrees, a dependency disappears, or an auditor asks why—because that is when the platform earns authority.

## External foundations

These sources supplied the primary risk-data and market-risk methodology. My resume is linked only to establish employment chronology.

| Source | How I applied it |
|---|---|
| [Basel Committee — Principles for effective risk data aggregation and risk reporting (BCBS 239, 2013)](https://www.bis.org/publ/bcbs239.htm) | I used its accuracy, completeness, timeliness, adaptability, and governance principles to design the shared risk model and evidence plane. |
| [Basel Committee — Revised market-risk framework (2016)](https://www.bis.org/press/p160114.htm) | I used its expected-shortfall, stress, and liquidity-horizon context to frame transaction and portfolio gates. |
