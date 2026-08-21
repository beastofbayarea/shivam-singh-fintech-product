# Owning the merchant after the terminal arrived

A shipped device was not an activated merchant, and an activated merchant was not yet a profitable relationship.

During my June–December 2023 Rakuten role, I led the merchant operating model for Rakuten Pay Terminal across merchants, sales, payments, finance, compliance, engineering, mobile, fulfillment, support, and product leadership.

Rakuten launched the terminal in July 2023 at ¥34,800 before tax / ¥38,280 including tax, with a zero-yen introduction campaign for qualifying new merchants. I corrected the retained internal ¥60,000 figure using the contemporaneous [official launch announcement](https://payment.rakuten.co.jp/news/2023072700/).

## The product was an operating relationship

The Android terminal combined card, contactless, e-money, and QR acceptance with a tablet, printer, mobile connectivity, and Wi-Fi. Rakuten’s [project history](https://payment.rakuten.co.jp/en/recruitment/innovation-culture/rakuten-pay-terminal-project/) describes it as both device consolidation and a gateway to merchant applications.

The decision was therefore not whether free hardware increased signups. It was whether a zero-upfront offer could create sustained payment activity, supportable operations, and cumulative contribution.

I wrote the cohort P&L before scale:

**payment contribution + connectivity/service contribution + later service contribution − device − shipping − onboarding − support − fraud/chargeback − servicing**

The investment gate was months to cumulative contribution breakeven. The model reached device-subsidy recovery in 14 months and 3.2× lifetime value. A 90-day pilot could not observe either; both remained forecasts pending mature cohorts.

## Two clocks governed launch

### Approval clock

Business/owner information, identity evidence, merchant review, and payment acceptance. Clear standard cases could use document extraction and rules. Low-confidence, mismatch, unusual-industry, or elevated-risk applications went to a person.

### Value clock

Device delivered, connectivity working, payment methods enabled, and first successful transaction completed.

The old route took 14 days to active. The redesigned path reached roughly 48 hours—12 days faster and 85.7% lower. First payment within 48 hours became a leading signal: fast starters were three times as likely to remain active at six months. That relationship is useful for intervention but not causal proof; motivated or prepared merchants may activate faster and retain better.

## The offer had an economic control

Project notes set a ¥200,000 monthly processing threshold and a return-or-pay rule after two under-threshold months. Public launch material confirms the zero-yen campaign had operating conditions but does not establish that exact threshold. I present ¥200,000 as the project design, not a universal Rakuten term.

The purpose was not punitive clawback. It was to align the subsidy with merchants capable of using the product and to trigger support/recovery before an inactive device became sunk cost.

## Fifty merchants proved the workflow; 500 tested the cohort

The first 50 merchants exposed provisioning, connectivity, review, shipping, exception, and first-payment failure modes. Only after those paths stabilized did the Osaka cohort expand to 500.

I made every function own a lifecycle state:

**applied → approved → provisioned → activated → qualified → retained → expanded**

Sales shared the six-month active metric instead of receiving only signup credit. Finance watched subsidy recovery rather than hardware margin. Compliance retained exception authority. Engineering and operations could not declare a shipped box done. Support owned contextual intervention before the merchant became dormant.

Cross-sell came only after the payment product worked. The terminal’s app surface could widen the relationship, but a service bundle could not rescue weak core acceptance or reliability.

## Cohort evidence and what remained modeled

| Measure | Baseline → target → recorded result | Method/boundary |
|---|---|---|
| Time to active | 14 days → ≤48 hours → ~48 hours | Completed eligible application to first successful transaction |
| 30-day activation | zero on new cohort → high majority → 72% | Activated / enrolled; treatment of rejected applicants not retained |
| Six-month activity | new cohort → sustained use → 81% | Denominator may be enrolled or activated and must be recovered |
| Early signal | baseline absent → identify intervention trigger → first-48-hour payers 3× as likely active at month 6 | Observational association |
| Payment volume | one-time-buyer cohort → higher subscriber usage → +40% | Cohort comparison; merchant size/category/motivation may differ |
| Device payback | no subsidy recovery → acceptable horizon → 14 months modeled | Cumulative contribution, not observed in 90 days |
| LTV | cohort baseline 1.0× → improve relationship value → 3.2× modeled | Retention and contribution assumptions, not six-month realized value |

Current company statements about tens of thousands of stores and later app expansion validate direction but postdate my project and are not my results.

I owned the service proposition, P&L model, approval/value clocks, activity control, 50-to-500 learning sequence, lifecycle accountability, leading indicators, and scale criteria. Risk/compliance owned merchant decisions; payments owned acceptance; hardware/software owned reliability; finance owned contribution; sales/support owned interactions.

The change was conceptual and operational: stop managing hardware distribution and start managing a merchant cohort. Once sustained processing paid for the device, onboarding, connectivity, first value, support, retention, and future services became one product.
