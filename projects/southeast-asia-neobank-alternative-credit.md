# Extending credit without treating a thin file as a bad customer

Roughly 70% of the target group had little or no formal credit history, and bureau-led approval was below 10%. Rejecting them revealed missing data, not necessarily high risk. Approving them without bounded exposure would have been equally irresponsible.

At McKinsey, I designed the product system for a Southeast Asian digital-bank launch across customers, bank Product/Risk, Data Science, regulators, telco/identity partners, Compliance, Servicing, Collections, and super-app/commerce channels.

The product had to solve three models at once: eligibility, first exposure, and economic distribution.

## Model one — eligibility with limits on data use

More than 400 candidate telco and behavioral features entered governance, not automatic approval. Each required a permitted purpose, stability window, missing-value treatment, expected relationship to risk, gaming test, fairness review, and correction owner.

Account tenure, top-up regularity, and long-run usage stability could be informative. Device price, granular location, and raw wealth-like measures were excluded or challenged when they acted as social/income proxies without enough incremental value. Sudden pre-application behavior spikes triggered review.

The bank received derived features, not unnecessary raw communication or movement history. Consent was explicit and reversible. Revocation stopped future use; records already involved in a decision followed legal/audit rules.

The decision output explained approve, decline, or limited entry. “No bureau hit” became insufficient evidence, not a negative character judgment.

## Model two — earn exposure from observed behavior

Alternative-data confidence did not justify a large unsecured limit. I defined a ladder:

**transaction account → small first limit → observe repayment/fraud → raise, hold, or reduce**

About 15% of users lacked sufficient telco history and entered a 30–60-day internal-observation path before reassessment. This created a product for the no-data customer while bounding early loss.

Approval and loss were monitored by model version, region, customer segment, channel, feature availability, and limit band. Fairness review included approval, false rejection, explanations, repayment outcomes, and access to the limited route; equal approval alone was not proof of fairness.

## Model three — acquire inside a useful habit

Paid alternatives in the source exceeded $100 per customer, incompatible with a sub-$10 goal. Discovery and consent were embedded in telco, ride-hailing/super-app, and commerce moments where people already paid, sold, traveled, or topped up.

Distribution partners owned more than signup:

- identity and consent completion;
- approval and activation;
- first useful payment;
- support and complaints;
- repayment and early delinquency by channel;
- acquisition cost per active served customer.

The 2016 [CPMI–World Bank financial-inclusion report](https://www.bis.org/cpmi/publ/d144.htm) emphasized adoption and use of a useful transaction account. That made payments the recurring product foundation rather than treating credit as a one-off lead.

## Bounded launch, not borrowed regulatory certainty

The launch tested eKYC/liveness, consent, feature use, explanations, fraud, fairness, exposure caps, complaints, and monthly drift within a controlled perimeter.

The retained source calls it a “regulatory sandbox.” The Monetary Authority of Singapore issued a sandbox consultation in June 2016, at the end of my role; that is relevant methodology but does not prove participation or geography. I preserve the bounded test without inventing a regulator or license.

[FATF’s 2013 mobile/internet payment guidance](https://www.fatf-gafi.org/content/dam/fatf-gafi/guidance/Guidance-RBA-NPPS.pdf.coredownload.pdf) supplied a period-appropriate risk-based control reference. The [World Bank Global Findex 2014](https://www.worldbank.org/en/news/feature/2015/04/20/global-findex-2014-unveils-worlds-most-comprehensive-set-of-data-on-financial-inclusion) supplied market context, not private model proof.

## Four outcomes moved together

| Product outcome | Baseline → target → recorded result | Measurement |
|---|---|---|
| Active customers | 0 → 100,000 in 90 days → >100,000 | Deduplicated users completing the activity definition; exact window not retained |
| Approval | <10% → widen responsible access → >40% | Approved / completed eligible applications; >30 points and >4× |
| CAC | paid benchmark >$100 → <$10 → <$10 | Attributable acquisition spend / active served customers; denominator must be recovered |
| NPL | no seasoned baseline → within risk appetite → 2.4% early indicator | Non-performing balance / outstanding launch balance; delinquency and seasoning absent |
| No-history route | none → safe path → ~15% of users | Users entering 30–60-day route / eligible onboarded users |

The 2.4% NPL figure cannot validate lifetime risk within a 90-day launch; credit losses season, and NPL definitions vary. Sub-$10 CAC is meaningful only if it refers to an identity-complete, active customer—not free registration.

The thesis, feature-governance system, thin-file/no-data journeys, graduated limits, partner economics, bounded release, scorecard, and stakeholder settlement defined my product authority. Data Science estimated; Risk set policy/limits; Compliance/regulators approved; partners supplied data/identity/distribution; Servicing/Collections carried outcomes.

This was not an alternative-data trick. It was a full inclusion product in which consented evidence established eligibility, a small exposure established trust, observed repayment expanded access, and embedded utility made the economics sustainable.
