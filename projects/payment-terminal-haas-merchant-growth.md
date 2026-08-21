# Turning a Payment Terminal into an Active-Merchant Service

I led this work during my [Rakuten experience from June to December 2023](https://github.com/beastofbayarea/shivam-singh-fintech-product/blob/main/shivam-singh-fintech-product.pdf).

The terminal simplified a merchant's countertop, but a ¥60,000 upfront price and paper-based KYC kept many merchants from becoming users. The organization was also measuring the wrong finish line. A shipped device created revenue once; an activated merchant processing payments created an ongoing relationship.

I redesigned the proposition as a zero-upfront hardware-as-a-service offer and made six-month merchant activity the governing measure.

## The economics began at the device subsidy

Removing the purchase price made adoption easier, but it transferred risk to the business. I modeled the cumulative contribution from the terminal subsidy, connectivity, payment revenue, service cost, activation, and retention. The model showed what processing behavior was needed to recover the device cost and when the cohort became contribution-positive.

I tied the offer to minimum processing activity. A merchant that did not reach the threshold had to return or pay for the device. This protected the zero-upfront experience from becoming an unbounded hardware giveaway.

The World Bank's Fast Payments Toolkit influenced how I considered merchant acceptance, interoperability, pricing, access, and consumer protection as one system. PCI DSS 4.0 provided the payment-data security and validation foundation.

## I redesigned activation around the clear case

Paper-based KYC made time to active stretch to 14 days. I automated provisioning and standard KYC cases, while sending low-confidence, mismatched, or unusual applications to a person.

That division improved speed without pretending every applicant had the same risk. The first 50 merchants tested the provisioning and review flow. I then expanded to a 500-merchant Osaka cohort to test the complete lifecycle: acquisition, KYC, shipment, first successful transaction, ongoing volume, support, retention, and subsidy recovery.

## One metric aligned six teams

Payments, Sales, Finance, Compliance, Engineering, Mobile, and Operations had different definitions of launch success. I gave the program two connected measures: time to first successful transaction and the percentage of merchants still active after six months.

Devices shipped became an input. Those two measures showed whether the experience worked for the merchant and whether the economics worked for the business.

## What the cohort showed

- Time to active fell from 14 days to about 48 hours.
- Seventy-two percent of merchants activated within 30 days.
- Eighty-one percent remained active after six months.
- Subscriber payment volume was 40% higher than for one-time buyers.
- Lifetime value increased 3.2 times.
- The device subsidy was recovered in 14 months.

Company-level figures such as total merchant locations and division growth provide useful context, but I do not present them as terminal-attributable impact. The cohort and lifecycle measures above are the direct evidence I use.

## The product shift that mattered

Hardware-as-a-service was not simply a financing change. It forced the team to own the entire merchant journey after shipment. When the business earns value from sustained processing, onboarding quality, first-use speed, support, reliability, and retention all become part of the product.

That is why I measure active customers and cumulative contribution rather than the moment an object leaves the warehouse.

## External foundations

These sources supplied the primary payments and security methodology. The resume link establishes employment chronology only.

| Source | How I applied it |
|---|---|
| [World Bank — Fast Payments Toolkit (2021)](https://fastpayments.worldbank.org/sites/default/files/2021-11/Fast%20Payment%20Flagship_Final_Nov%201.pdf) | I used its merchant-acceptance, pricing, interoperability, access, and consumer-protection framework to design the service model. |
| [PCI Security Standards Council — PCI DSS 4.0 release (2022)](https://www.pcisecuritystandards.org/about_us/press_releases/securing-the-future-of-payments-pci-ssc-publishes-pci-data-security-standard-v4-0/) | I used its payment-account-data control principles as activation and operations requirements. |
