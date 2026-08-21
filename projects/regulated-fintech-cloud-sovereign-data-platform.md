# Regulated FinTech Cloud - Sovereign Data Platform

## What I worked on

I completed this work during my [Microsoft experience from January 2020 to August 2022](https://github.com/beastofbayarea/shivam-singh-fintech-product/blob/main/shivam-singh-fintech-product.pdf).

I productized two linked regulated-cloud needs under the Microsoft FinTech role: a time-critical trading workload and a ten-market sovereignty launch. Performance SLOs, jurisdiction rules, regional data controls, and audit evidence became a reusable financial-services deployment pattern.

## At a glance

- I recovered a regulated trading workload from six-hour reconciliation to 480 ms, saving and expanding a cloud contract from $5M to $7M.
- I replaced a centralized architecture carrying $25M in regulatory exposure with automated regional pods for ten jurisdictions.
- I reduced reporting time from two hours to ten minutes, lowered reporting CPU roughly 40%, and launched all ten markets with clean audits.

## The situation

One financial-services client treated critical trading and routine reporting as equal queue traffic; another attempted to move regulated European and Chinese data through a U.S.-hosted monolith.

## What I needed to accomplish

I needed to define the product requirements and launch gates needed to meet hard performance and jurisdiction constraints while preserving global operational visibility and a repeatable deployment mechanism.

## What I did

- I prioritized preemptive fast lanes for trade and risk work while moving reporting to a separate serverless path.
- I defined jurisdiction-specific requirements for compute, storage, encryption, consent, retention, and audit controls.
- I productized WORM retention, customer-managed HSM keys, and row-level cross-border permission checks as reusable platform capabilities.
- I limited cross-region reporting to approved, de-identified signals so customers retained global risk insight without exporting identity data.

## The results

- Critical-query latency reached 480 ms.
- Reporting fell to ten minutes and supported 500 concurrent analysts.
- Ten sovereign deployments launched with zero audit exposure.
- The renewed contract expanded to $7M.

## Decisions and trade-offs

- I standardized deployment automation and evidence while allowing jurisdiction-specific policy.
- I paused the multi-market launch when the centralized design became legally unsafe.
- I preserved global risk visibility through de-identification rather than identity export.

## How I led

I aligned product, architecture, security, compliance, client, and commercial teams around explicit SLO and jurisdiction gates, turning regulatory constraints into reusable financial-services product requirements.

## Why I chose this approach

I used [NIST - SP 800-53 Revision 5 (2020)](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final) to ground security, privacy, governance, supply-chain, and accountability framework. I used [NIST - Zero Trust Architecture (2020)](https://doi.org/10.6028/NIST.SP.800-207) to ground least-privilege and per-resource access model.

## Sources and external context

I used independent methodology and market evidence to shape the work. The resume link above is included only to establish the employment timeline.

| Source | How it informed my work | Timing |
|---|---|---|
| [NIST - SP 800-53 Revision 5 (2020)](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final) | I used it to ground security, privacy, governance, supply-chain, and accountability framework. | — |
