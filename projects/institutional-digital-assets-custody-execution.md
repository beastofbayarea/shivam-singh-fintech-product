# Keeping institutional digital assets in custody when the client needed to trade

The platform held assets safely and lost the highest-value moment.

Wallet-flow analysis indicated that roughly 70% of targeted institutional outflows went to competitor execution venues. Clients trusted custody but could wait up to 24 hours to move a cold asset, so urgent trades and fees left the relationship.

During my D. E. Shaw role, I set the product strategy across institutional clients, Custody Operations, Trading, Treasury, Risk, Compliance, Engineering, Sales, and Finance. The leak became a controlled bridge between two products that still had to remain operationally distinct.

## The metric was client share of wallet, not market volume

Rising crypto prices could lift every venue. I defined the business measure as:

**captured execution volume on the proposed service / total observable execution volume for the client**

It excluded opaque off-chain or prime-broker activity, but it was closer to the product problem than total market volume.

I then ranked requests by observed outflow, tagged lost economics, urgency, implementation risk, and balance-sheet exposure. The sequence became:

1. test pricing with high-churn clients;
2. close the custody-to-trade timing gap;
3. expose institutional accounts/sub-accounts via API;
4. join custody and execution economics;
5. expand asset breadth only after credit and operations held.

NFT and DeFi breadth stayed behind reliability because they had less evidenced blocked value and more unresolved risk.

## Ten clients established routing demand

Ten high-churn institutions entered a 30-day shadow-pricing pilot with lower maker–taker rates and credits. Trading volume increased 400%—five times baseline—while observed outflows to targeted competitors fell close to zero.

The cohort already held assets on-platform, which made the test stronger than a generic market pre/post. It was still selected, non-random, and bundled price with service change. I used the result as willingness-to-route evidence, not a clean elasticity coefficient.

## Instant access came from credit, not pretending custody moved instantly

The product created trading credit against verified, segregated assets:

**eligible custody assets × haircut − obligations − concentration reserve = available trading credit**

Before exposure, the service checked asset eligibility, valuation freshness, volatility haircut, client limit, concentration, settlement path, and authorized sub-account. Credit became available in under one second while cold assets remained under custody controls.

An illustrative “$100 million credit against $100 million custody” appears in design notes. I do not claim a live 100% advance rate; volatile collateral requires lower haircuts, eligible asset classes, hedging, or other protection.

Early concentration led us to dynamic haircuts, risk-based pricing, eligibility gates, and lower limits for unpredictable flows. The objective was immediate bounded access, not zero wait at any balance-sheet cost.

## One proposition, four control domains

**Custody** retained segregation, key, withdrawal, and audit controls.

**Credit** owned valuation, haircut, exposure, concentration, margin, and liquidation.

**Execution** owned orders, market access, price, surveillance, and venue behavior.

**Settlement** reconciled obligations to custody and credit records.

Commercially, trading fees could offset custody fees. Operationally, no netting could erase evidence or transfer authority between domains.

The [CFTC’s 2017 virtual-currency primer](https://www.cftc.gov/PressRoom/PressReleases/7631-17) and [NIST’s 2018 blockchain overview](https://doi.org/10.6028/NIST.IR.8202) provide period-appropriate context for custody, keys, ledgers, and off-chain dependencies. They do not establish licenses or validate this pilot.

## What the pilot supports

- **Competitor leakage:** ~70% of targeted observable outflows → materially recapture → close to zero during the selected pilot. Method: known wallet/venue flows for the same ten-client cohort.
- **Trading volume:** baseline index 100 → test material route change → 500 after 30 days. Method: comparable client volume; +400%.
- **Access:** up to 24 hours → immediate bounded availability → <1 second. Method: request to approved execution credit—not cold-asset movement or final settlement.
- **Share of wallet:** low → materially improve → exact result absent. Method: captured / observable client execution volume.

The source also contains 2021 public-looking volume and revenue metrics that postdate my December 2019 departure and a McKinsey variation. I exclude them and present this as a product strategy/pilot, not ownership of a later public custody company.

My scope covered leakage diagnosis, share-of-wallet measurement, the economic backlog, pricing pilot, custody-to-credit proposition, API/sub-account requirements, commercial flywheel, and concentration response. Custody, Treasury, Risk, Compliance, Engineering, and Trading retained approval/operations; licenses, legal entity, and agreements remained separate gates.

The strategic product insight was that trust can create a moat and a trap. Custody retained the client only until the next urgent job; a governed credit bridge let the platform serve that moment without weakening the custody boundary that earned trust in the first place.
