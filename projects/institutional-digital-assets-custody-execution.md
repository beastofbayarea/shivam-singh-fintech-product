# Keeping Institutional Digital Assets in Custody When the Client Needed to Trade

I led a product strategy for institutions that wanted to trade digital assets without moving them out of trusted custody. I had identified that clients lost time and the platform lost trading business because custody and execution were separate services. I worked with institutional clients, custody operations, traders, risk, compliance, treasury, engineering, sales, and finance.

This project is assigned to my D. E. Shaw role from July 2016 to December 2019. The underlying source page also contains a “McKinsey” variation and public-looking 2021 custody-company metrics that postdate the role. D. E. Shaw describes itself as an investment and technology development firm, not a public digital-asset custodian. I therefore reconstruct the work as a product strategy/pilot and exclude the later company figures rather than imply ownership of another company's results.

## The observable leak

Blockchain and wallet-flow analysis indicated that about 70% of targeted institutional outflows went to competitor execution venues. The client trusted the custody control but could wait as long as 24 hours for an asset movement from cold storage, so urgent trading activity and fees left the platform.

Total crypto volume was a poor measure because a rising market could lift every venue. I chose **share of each client's observable execution wallet**:

`execution volume captured on proposed service ÷ total observable execution volume for that client`

This did not reveal all off-chain or prime-broker activity, but it was closer to the business problem than market-wide volume.

## I turned requests into blocked economics

Sales wanted API sub-accounts, lower fees, instant liquidity, and speculative asset expansion. I ranked them by observed outflow, tagged lost opportunity, client urgency, implementation risk, and balance-sheet exposure.

The first sequence was:

1. prove price elasticity with existing high-churn clients;
2. remove the custody-to-trade time gap;
3. expose institutional account and execution controls through APIs;
4. join custody and trading economics;
5. expand assets only after operational and credit controls held.

NFT and DeFi breadth stayed behind trading reliability because it had less evidenced blocked revenue and more unresolved risk.

## The pricing test

Ten high-churn institutions entered a 30-day shadow-pricing pilot using lower maker–taker rates and fee credits. Pilot trading volume increased 400%, meaning five times the baseline level, while observed outflows to targeted competitor venues fell close to zero.

The design was more persuasive than a simple pre/post comparison because the clients and custodied assets were already present. It still was not randomized: the cohort was selected for churn, the offer bundled price and service changes, and market conditions could alter trading demand. The result established strong willingness-to-route evidence, not a clean elasticity coefficient.

## The instant-credit product

Instead of moving cold assets into a hot execution wallet before every trade, the design created trading credit against verified, segregated custody assets.

`eligible custodied assets × haircut – existing obligations – concentration reserve = available trading credit`

Sub-accounts separated strategies and authorized users. Pre-trade checks validated asset eligibility, valuation freshness, volatility haircut, client limit, concentration, and settlement path. The execution balance could become available in under one second while the custody asset remained subject to its control process.

“Up to $100 million of credit against $100 million of custody” appears in the design notes as an illustrative maximum. A 100% advance rate would be inappropriate for volatile collateral without eligible assets, stablecoin/cash treatment, hedging, or other protection. I do not present that example as the live limit.

Early concentration under volatile conditions led to dynamic haircuts, risk-based pricing, eligibility gates, and lower limits for less predictable flows. The product objective was not zero transfer time at any balance-sheet cost; it was immediate, bounded access for clients whose collateral and behavior supported it.

## Custody and execution remained separate control domains

The flywheel joined the customer proposition without blurring responsibilities:

- custody retained segregation, key, withdrawal, and audit controls;
- credit owned collateral valuation, haircut, exposure, liquidation, and concentration;
- execution owned orders, market access, price, and surveillance;
- settlement reconciled execution obligations against the custody/credit record;
- commercial logic could credit trading fees against custody fees without netting away control evidence.

The CFTC's 2017 virtual-currency primer is the period-appropriate market reference. NIST's 2018 blockchain overview informs keys, ledgers, consensus, and off-chain dependencies. Neither source converts a strategy pilot into a licensed custody or exchange business.

## Evidence I retain

| Claim | Baseline | Result | Qualification |
|---|---:|---:|---|
| observed outflows to competitor execution | ~70% of targeted outflows | close to zero in pilot | on-chain/known venues only; selected cohort |
| pilot trading volume | pre-offer client volume | +400% / 5× | 30 days, 10 clients, price and product bundled |
| time to execution access | up to 24 hours | <1 second | credit availability, not movement of cold asset or final settlement |
| share of wallet | low because execution left | materially recaptured | exact denominator/result not retained |

I exclude the source page's 2021 institutional-volume and services-revenue figures because they postdate the role and appear to describe a broader public company. I also do not call competitor outflows “zero” when the retained phrasing is “close to zero.”

I owned the outflow diagnosis, economic backlog, pilot design, custody-to-credit proposition, API/sub-account requirements, commercial flywheel, and risk-control response. Custody, Treasury, Risk, Compliance, Engineering, and trading owners retained their approvals and operations. A regulated launch, legal entity, licenses, and client agreements would have been separate gates beyond product strategy.

The strategic lesson is not that custody should become an exchange. It is that a trusted product can lose the customer's highest-value moment unless it offers a governed bridge to the next job.

Relevant period sources: [CFTC LabCFTC Virtual Currency Primer, October 2017](https://www.cftc.gov/PressRoom/PressReleases/7631-17), [NIST IR 8202, *Blockchain Technology Overview*](https://doi.org/10.6028/NIST.IR.8202), and [D. E. Shaw's description of its investment and technology business](https://www.deshaw.com/what-we-do).

