# Extending Credit Without Treating a Thin File as a Bad Customer

I led the alternative-credit product for a Southeast Asian digital bank launch during my McKinsey role. I had identified that people without bureau histories were being rejected before the bank could observe whether they could repay, while customers and regulators needed limits on how mobile behavior affected a financial decision. I worked with prospective customers, bank product and risk leaders, data scientists, regulators, telco and identity partners, Compliance, servicing and collections teams, and super-app and commerce channels.

The work occurred from July 2014 to June 2016. Roughly 70% of the target group had little or no formal credit history, and bureau-led approval was below 10%. The product needed to solve three coupled models: **eligibility**, **first exposure**, and **economic distribution**.

## Model one: eligibility without data overreach

The underwriting design used more than 400 derived telco and behavioral variables. Quantity was not the point. Each candidate signal needed a permitted purpose, stability window, missing-value treatment, expected risk relationship, gaming test, fairness review, and correction owner.

Useful classes included account tenure, top-up regularity, and long-run usage stability. I excluded or challenged device price, fine-grained location, and raw wealth-like measures when they operated as social or income proxies without enough incremental risk value. A sudden behavior spike immediately before an application triggered review rather than reward.

The bank received derived features rather than unnecessary raw communication content or movement history. Consent was explicit and reversible; revocation stopped future use, while legal and audit requirements governed records already used for a decision.

No bureau hit became “insufficient evidence,” not “bad credit.” The model produced reasons for approve, decline, or limited entry so Risk and a customer-support path could inspect the decision.

## Model two: earn a larger limit from observed repayment

A high score based on alternative data did not justify an immediately large unsecured exposure. I defined a graduated product:

`limited account/payment access → small first credit limit → observe repayment and fraud → raise, hold, or reduce limit`

About 15% of users lacked enough telco history and entered through a 30–60 day internal-observation path before reassessment. That created an inclusion route for the no-data customer while bounding first loss.

The decision policy monitored approval and loss by model version, region, income segment, channel, feature availability, and limit band. Fairness review compared selection and outcomes but did not assume equal approval alone proved fairness; repayment performance, false rejection, explanations, and access to the limited path also mattered.

## Model three: acquire inside a useful financial habit

Paid media benchmarks in the source page exceeded $100 per customer, incompatible with a sub-$10 target. I embedded discovery and consent in telco, ride-hailing/super-app, and commerce journeys where customers already paid, sold, traveled, or topped up.

The distribution partner was accountable beyond signup:

- identity completion and consent quality;
- approval and activation;
- first useful payment;
- support and complaint handoff;
- repayment and early delinquency by channel;
- acquisition cost per active, served customer.

The April 2016 CPMI–World Bank report made the period-appropriate product point: financial inclusion depends on adoption **and use** of a useful transaction account. Credit embedded in payments and commerce had more recurring utility than an isolated loan lead.

## The regulatory path was bounded, but the source overstates certainty

The launch used a bounded testing approach for eKYC and liveness, consent, alternative features, explanations, fraud, fairness, exposure caps, complaints, and monthly drift.

The source calls this a “regulatory sandbox.” Singapore's Monetary Authority issued its sandbox consultation in June 2016, at the end of the role period. That is valid contemporaneous methodology but does not prove this bank participated in the Singapore sandbox. I describe the operating controls and bounded launch without naming a regulator or license that the record does not substantiate.

FATF's 2013 mobile and internet payment guidance supports risk-based controls rather than maximum friction for every customer. World Bank Global Findex 2014 supplies the period market-access evidence. Neither source validates the private model's performance; that rests on the launch record.

## The four headline results must travel together

| Measure | Baseline | Target | Reported result | Measurement caveat |
|---|---:|---:|---:|---|
| active customers | zero | 100,000 in 90 days | >100,000 | activation event and deduplication not retained |
| approval | <10% | widen viable access | >40% | approved/eligible denominator needs recovery |
| CAC | paid path >$100 benchmark | <$10 | <$10 | must confirm whether denominator is approved, activated, or retained |
| NPL | no seasoned new-book baseline | within risk appetite | 2.4% | delinquency definition and vintage seasoning absent |

Approval increased by more than 30 percentage points and more than fourfold. That is only healthy expansion if identity, fraud, repayment, complaints, and customer outcomes remain inside their bounds.

The 2.4% NPL measure cannot fully validate a 90-day launch. Credit losses season over time, and “NPL” may mean 30, 60, or 90 days past due depending on the institution. I treat it as an early reported portfolio indicator, not lifetime expected loss.

Likewise, sub-$10 CAC is compelling only if the denominator is a customer who completed identity, activated, and could use the account. A free registration is not an acquired banking relationship.

## What I owned

I owned the product thesis, feature-governance requirements, thin-file and no-data paths, graduated-limit policy, partner-distribution economics, bounded launch record, cross-functional alignment, and scorecard. Data Science owned model estimation; Risk owned credit policy and limits; Compliance and regulators owned approval; partners supplied identity, data, and distribution under defined contracts; Operations and Collections owned customer outcomes after decision.

The work was not a credit-model hack. It was a system in which consented evidence could establish eligibility, a small product could establish trust, and embedded distribution could make the economics work—without converting “financial inclusion” into a license to approve blindly.

Period references: [World Bank Global Findex 2014 launch](https://www.worldbank.org/en/news/feature/2015/04/20/global-findex-2014-unveils-worlds-most-comprehensive-set-of-data-on-financial-inclusion), [CPMI–World Bank, *Payment aspects of financial inclusion*, April 2016](https://www.bis.org/cpmi/publ/d144.htm), [FATF risk-based guidance for mobile and internet payments, June 2013](https://www.fatf-gafi.org/content/dam/fatf-gafi/guidance/Guidance-RBA-NPPS.pdf.coredownload.pdf), and the [MAS sandbox consultation, June 2016](https://www.nas.gov.sg/archivesonline/data/pdfdoc/20160606006/Media%20release%20-%20Public%20Consultation%20on%20Sandbox%20Guidelines_FINAL.pdf).

