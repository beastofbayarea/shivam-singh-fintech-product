# Extending Digital-Asset Custody into Institutional Execution

I did this work during my [D. E. Shaw experience from July 2016 to December 2019](https://github.com/beastofbayarea/shivam-singh-fintech-product/blob/main/shivam-singh-fintech-product.pdf).

Institutions trusted the platform to hold assets, but they moved those assets to competing venues whenever they needed immediate liquidity. Roughly 70% of institutional outflows followed that pattern. The business retained the custody responsibility while competitors captured trading volume and economics.

I set out to make custody the starting point of an execution relationship without weakening the controls that had earned institutional trust.

## The useful metric was share of wallet

Total crypto-market volume could rise enough to make almost any pilot look successful. I therefore measured how much of each institution's trading activity the platform captured and how much value still flowed to competitors.

I converted sales requests into a blocked-revenue backlog. Instant access to liquidity, institutional APIs, and commercial pricing ranked above speculative feature expansion because they addressed observable outflow behavior.

The CFTC's 2017 primer gave me the contemporaneous market and risk context for virtual currencies. NIST's blockchain overview provided the technical foundation for ledgers, keys, consensus, custody, and system limitations. I used both to keep the product conversation anchored in operational and market risk, not just trading demand.

## A 30-day pilot tested the commercial mechanism

I selected ten institutions with high churn and ran shadow pricing for 30 days. The cohort let me compare expected and observed share-of-wallet behavior before changing the broader pricing model.

Lower maker-taker pricing and fee credits increased pilot volume 400%, while targeted competitor outflows fell close to zero. Because the measure was within-client share rather than market growth, the result gave me stronger evidence that the product and pricing bundle had changed behavior.

## Credit removed the 24-hour delay

Moving assets out of cold storage could take as long as 24 hours, which made the custody product unusable for time-sensitive execution. I designed instant trading credit against segregated custody assets, supported by API sub-accounts.

The credit preserved asset segregation while reducing time to trade to under one second. When early use revealed concentration risk, I added client eligibility, volatility-sensitive limits, and risk-based pricing. The goal was not maximum volume; it was faster access inside a bounded balance-sheet exposure.

## What changed

- Pilot trading volume increased 400%.
- Targeted competitor outflows declined to almost zero.
- Time to trade fell from as much as 24 hours to under one second.
- The combined custody, liquidity, execution, and pricing proposition created a stronger retention mechanism.

Broader company results later showed institutional activity and services revenue expanding, but I keep those figures separate from my direct evidence. The ten-client cohort, observed outflows, pilot volume, and access time are the measures I use for this work.

## My takeaway

A trusted product can still lose the most valuable part of the customer journey. I look for that handoff and ask whether the platform can extend into it without compromising the reason customers trusted the original product.

Here, the answer was not to blur custody and trading risk. It was to connect them through explicit collateral, eligibility, limits, pricing, and APIs—creating a custody-to-execution loop with controls visible to both the client and the risk team.

## External foundations

The following sources supplied the primary contemporaneous market and technical context. The resume link establishes employment chronology only.

| Source | How I applied it |
|---|---|
| [U.S. Commodity Futures Trading Commission — Primer on Virtual Currencies (2017)](https://www.cftc.gov/PressRoom/PressReleases/7631-17) | I used it to frame market structure, volatility, custody, and operational risk in the period of the work. |
| [NIST — Blockchain Technology Overview (2018)](https://doi.org/10.6028/NIST.IR.8202) | I used its treatment of ledgers, consensus, keys, and limitations to define the technical and control boundaries. |
