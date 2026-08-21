# Building Credit Access for Customers Without Bureau Histories

I worked on this Southeast Asian neobank during my [McKinsey experience from July 2014 to June 2016](https://github.com/beastofbayarea/shivam-singh-fintech-product/blob/main/shivam-singh-fintech-product.pdf).

Roughly 70% of the target population lacked a formal credit history. Traditional bureau-led underwriting therefore approved fewer than 10% of applicants. Paid acquisition was also uneconomic, and regulators reasonably expected a credible approach to identity, privacy, fraud, explanation, and portfolio loss.

I treated the absence of a bureau file as a missing signal—not proof that the customer was uncreditworthy.

## I designed the data boundary before the score

The product used consented telco behavior across more than 400 derived variables. I focused on long-term consistency and stability, not wealth proxies. Sudden behavior changes immediately before an application were routed for review because they could indicate manipulation or fraud.

I minimized the data entering the underwriting system. The product received the derived signals needed for the decision rather than unnecessary raw personal records, and consent remained reversible.

The World Bank's 2014 Global Findex provided the market foundation for access gaps, mobile accounts, and digital payments. FATF's risk-based guidance for mobile and internet payments influenced the control design: identity and monitoring effort should respond to observed risk rather than make every user pass the maximum-friction path.

## Approval and fairness were reviewed together

I tested whether variables behaved as hidden income or protected-trait proxies and removed those that created unfair separation without a defensible risk relationship. The score produced explanations that could support review and customer communication.

Uncertain applicants were not forced into a binary full-credit-or-rejection choice. I started them with a limited product and graduated limits as repayment evidence accumulated. That bounded the first-loss exposure while allowing the platform to learn from the customer's own behavior.

## Distribution was embedded in an existing habit

Acquiring each customer through paid media would have broken the unit economics. I placed discovery and signup inside telco, super-app, and commerce ecosystems where the target customer already completed frequent tasks.

The BIS and World Bank work on payment aspects of financial inclusion reinforced the importance of a useful transaction account and accessible payment infrastructure. Credit was more sustainable when it sat inside a recurring financial relationship rather than appearing as an isolated loan offer.

## The regulatory pathway was part of the product

I worked through a bounded sandbox process that covered eKYC, consent, explanations, bias tests, fraud controls, customer safeguards, and monthly drift monitoring. Each expansion decision considered approval, acquisition cost, loss, fairness, and operating readiness together.

## What the evidence showed

- Approval increased from below 10% to above 40%.
- The launch reached more than 100,000 active users in 90 days.
- Customer-acquisition cost remained below $10.
- The portfolio maintained a 2.4% non-performing-loan ratio.

## The product principle I carried forward

Financial inclusion is not achieved by maximizing approvals. It requires a product that creates access, earns repayment evidence over time, protects customer agency, and keeps portfolio quality inside an explicit boundary. I design the data, credit limit, distribution, and regulatory pathway as one system because weakening any one of them eventually weakens the others.

## External foundations

These sources supplied the primary market, payments, and risk-control methodology. My resume is linked only to establish employment chronology.

| Source | How I applied it |
|---|---|
| [World Bank — Global Findex 2014 launch (2015)](https://www.worldbank.org/en/news/feature/2015/04/20/global-findex-2014-unveils-worlds-most-comprehensive-set-of-data-on-financial-inclusion) | I used its evidence on account access, mobile accounts, and digital payments to frame the addressable inclusion problem. |
| [BIS and World Bank — Payment aspects of financial inclusion (2016)](https://www.bis.org/cpmi/publ/d144.htm) | I used its transaction-account and retail-payment framework to connect credit access to a recurring financial relationship. |
| [FATF — Risk-based approach to mobile and internet payments (2013)](https://www.fatf-gafi.org/content/dam/fatf/documents/recommendations/Guidance-RBA-NPPS.pdf) | I used its risk-based identity and monitoring principles to balance access with AML/CFT controls. |
