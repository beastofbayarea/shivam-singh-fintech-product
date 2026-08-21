# Owning the Merchant After the Terminal Arrived

I led a merchant-economics project for Rakuten Pay Terminal. I had identified that small businesses needed a simple way to start accepting digital payments, while Rakuten needed merchants to activate and keep processing rather than merely receive a device. I worked with merchants, Sales, Payments, Finance, Compliance, Engineering, Mobile, fulfillment, support, and product leadership.

Rakuten Pay Terminal launched in July 2023 during my June–December 2023 role. Rakuten's official launch announcement priced the terminal at ¥34,800 before tax, or ¥38,280 including tax, and offered qualifying new merchants a zero-yen introduction campaign. The retained internal project page says ¥60,000; because the primary company source is specific and contemporaneous, I corrected the product price instead of preserving the larger number.

## The terminal was already more than hardware

The all-in-one Android device combined card, contactless, electronic-money and QR acceptance with a tablet, printer, mobile connectivity and Wi-Fi. Rakuten's own project history says the product was intended to replace a separate tablet or phone, card reader, and Bluetooth printer, and to become a gateway for additional merchant applications.

The product question was therefore not whether to “give away a terminal.” It was whether a zero-upfront offer could produce an active, contribution-positive merchant relationship.

I owned the merchant operating model from acquisition through six-month retention and subsidy recovery. I wrote the cohort P&L, defined the activation and qualification clocks, sequenced learning from 50 merchants to a 500-merchant pilot, aligned six teams on one lifecycle, and set the evidence required before a zero-yen hardware offer could become a scalable payments-and-services relationship.

## I wrote the cohort P&L before scaling the offer

For each acquisition cohort, I modeled:

`payment contribution + connectivity/service contribution + later merchant-service contribution – device – shipping – onboarding – support – fraud/chargeback – servicing`

The governing economic measure was months to cumulative contribution breakeven. The retained model reached device-subsidy recovery in 14 months.

That is a forecast, not something a 90-day pilot could observe. The 500-merchant Osaka pilot supplied early activation and volume inputs; the 14-month payback and 3.2× lifetime value depended on retention and contribution assumptions that required later cohort evidence. I keep observed and modeled measures separate.

The zero-yen offer included an activity condition. The internal design notes describe a ¥200,000 monthly processing threshold and a return-or-pay rule after two under-threshold months. Rakuten's public launch announcement confirms that the zero-yen campaign had an operating condition, but the public page does not establish this exact threshold. I therefore present ¥200,000 as the project design, not a universal Rakuten term.

## Activation had two clocks

**Approval clock:** business and owner information, identity evidence, merchant review, and payment acceptance. Clear standard cases could use document extraction and rules; low-confidence, mismatched, unusual-industry, or elevated-risk cases went to a person.

**Value clock:** device delivered, connectivity working, payment methods enabled, and first successful transaction completed.

The first 50 merchants tested provisioning and exception behavior before the 500-merchant cohort. The old path took 14 days to active; the new path reached about 48 hours, an 85.7% reduction. A public Rakuten page now advertises merchant review and shipment in as little as three days each, which is current context—not evidence for or against the internal pilot's definition of “active.”

First payment within 48 hours was an especially useful leading indicator: those merchants were reported to be three times as likely to remain active at six months. Because fast starters may already be more motivated or operationally prepared, the relationship supports intervention and prioritization, not pure causality.

## Six teams received one lifecycle, not one launch date

| Merchant state | Product measure | Owner | Failure response |
|---|---|---|---|
| applied | complete eligible application | Sales/Product | guided correction |
| approved | review time and exception reason | Compliance | manual review or documented rejection |
| provisioned | device, connectivity, account ready | Engineering/Mobile/Ops | repair before shipment close |
| activated | first successful transaction | Payments/Support | contextual onboarding |
| qualified | sustained processing threshold | Finance/Sales | warning, recovery plan, return/pay path |
| retained | active at six months | all teams | diagnose volume, reliability, support, or fit |
| expanded | added apps/services | Product | value-led cross-sell only after core health |

Sales kept signing credit but shared the six-month active measure. Finance watched subsidy recovery rather than hardware margin. Compliance retained exception authority. Engineering and Operations could no longer call a shipped box a completed product.

## Cohort evidence

- **72% activated within 30 days.** The denominator appears to be enrolled merchants; the retained notes do not state whether rejected applications were excluded.
- **81% were active after six months.** The denominator—enrolled or activated merchants—must be recovered before funnel arithmetic.
- **Subscriber payment volume was 40% higher than for one-time buyers.** This is an observational cohort comparison; merchant size, category, and motivation could differ.
- **Modeled LTV was 3.2×.** It depends on retention, payment contribution, support and subsidy assumptions; it was not lifetime revenue observed in a six-month window.
- **Modeled device recovery was 14 months.** This was the investment gate, not a 90-day realized result.

The 500-merchant pilot was large enough to expose workflow and early behavior, but not to make a stable claim about lifetime economics. I would require cohorts by merchant category, pre-period processing, device status, fraud/chargebacks, contribution margin, support contacts, and survival before a national decision.

## Why the official market evidence matters

Rakuten states that tens of thousands of stores now use the terminal and that its app surface is intended to bring more Rakuten services into the merchant relationship. Those later company facts validate the strategic direction, but they are not attributed to my six-month project. Similarly, company-wide merchant locations, payments-division revenue, tourism, and cross-border commerce are context, not terminal-pilot impact.

I owned the service proposition, cohort economics, activation metric, usage-control design, 50- and 500-merchant learning sequence, cross-functional alignment, and scale criteria. Risk and Compliance owned merchant approval; Payments owned acceptance; hardware and software teams owned reliability; Finance owned contribution accounting; Sales and Support owned merchant interaction.

The shift was from shipping an object to operating a merchant. Once revenue depended on sustained payment activity, onboarding, connectivity, reliability, support, retention, and subsidy recovery all became one product.

### Primary product evidence

- [Rakuten Payment — July 2023 launch announcement](https://payment.rakuten.co.jp/news/2023072700/) provides the official launch date, ¥38,280 tax-inclusive price, product capabilities, and zero-yen campaign context.
- [Rakuten Payment — terminal project history](https://payment.rakuten.co.jp/en/recruitment/innovation-culture/rakuten-pay-terminal-project/) documents the device consolidation, field testing, Rakuten Mobile collaboration, later store scale, and app-platform direction.
- [Rakuten Pay Terminal current product page](https://pay.rakuten.co.jp/business/service/terminal/) is used only for current product context because pricing, review times, and campaigns change.
- [PCI DSS v4.0 release](https://www.pcisecuritystandards.org/about_us/press_releases/securing-the-future-of-payments-pci-ssc-publishes-pci-data-security-standard-v4-0/) supplied the payment-data control context.
