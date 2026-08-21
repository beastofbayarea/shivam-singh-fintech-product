# Shivam Singh — FinTech Product Management

## Tell me about yourself

**Q: Tell me about yourself / walk me through your background.**

**A:** I am a FinTech product leader who builds the infrastructure and customer experiences behind trusted financial decisions. I started at McKinsey in digital banking and product strategy, including alternative-credit and market-entry work for customers without conventional credit histories. That experience taught me to connect access and growth to consent, fraud, loss limits, regulatory sequencing, and unit economics from the beginning.

At D. E. Shaw, I worked on institutional products where speed and control had to coexist: real-time risk, digital-asset custody, execution, liquidity, and capital allocation. At Microsoft, I led FinTech cloud, payments, and compliance products, including workloads that combined sub-second operational requirements with market-by-market sovereignty and audit rules. During my MBA role at Rakuten, I reframed a payment terminal from a hardware sale into a merchant lifecycle product with activation, retention, payment-volume, and payback economics. At AWS, I have focused on financial-services platforms, including regulated agent workflows with identity, permissioned data and tools, human approval, traceability, and economic routing.

My background has progressed from market and credit strategy to real-time financial infrastructure and then to regulated automation at platform scale. I am strongest when the visible customer experience depends on difficult underlying decisions about authority, ledger truth, risk, liquidity, jurisdiction, or recovery. I own the product strategy and economic model while making the control path understandable enough to become a source of customer trust rather than friction.

A financial product is a promise backed by an operating system. The customer sees a payment, credit decision, trade, workflow, or account. Underneath it, identity, permissions, liquidity, ledger truth, risk policy, evidence, and recovery must agree.

I build that hidden system as part of the product—not as control work added after the experience is designed.

[Resume](./shivam-singh-fintech-product.pdf) · [LinkedIn](https://www.linkedin.com/in/beastofbayarea) · [shiv-fintech-product@umich.edu](mailto:shiv-fintech-product@umich.edu)

## The six contracts behind trustworthy financial products

### Permission to act

[Financial-services agents for regulated workflows](./projects/financial-services-agent-platform-regulated-workflows.md) established an authority chain from authentication and permitted evidence through consequence-based confirmation, execution, and trace. Six recurring blockers became one managed platform surface: knowledge, identity, tools, approval, observability, and cost. Comparable prototype-to-pilot work moved 40% faster; one lighthouse path fell from eight weeks to three days; grounded knowledge setup dropped to under five minutes. Model routing cut eligible routine-workflow cost by as much as 50%, while annual savings and support-capacity figures remained explicitly modeled.

The product question was never “Can the agent do it?” It was “Who allowed this action, against which evidence, with what limit, and how do we reverse or review it?”

### Permission to release capital

[The real-time risk gate](./projects/real-time-risk-capital-release.md) replaced fragmented retrospective checks with a common trade language, deterministic limits, explainable anomaly detection, degraded modes, and staged authority transfer. Risk-check latency moved from 90 milliseconds to 4.2 milliseconds, three-month shadow comparison reached roughly 98% agreement, false positives fell about 90%, and the system blocked $15 million of harmful exposure. The reported $85 million result is treated as internal risk or balance-sheet capacity, not mislabeled regulatory capital.

### Permission to use assets without breaking custody

[Institutional digital-asset custody and execution](./projects/institutional-digital-assets-custody-execution.md) began with an observable client problem: assets left custody when clients needed to trade. I designed instant, bounded execution credit against segregated assets rather than pretending cold assets could move instantly. Across a ten-client pilot, access fell from as much as 24 hours to under one second, targeted competitor leakage approached zero, and comparable trading volume rose fivefold. Custody, credit, execution, liquidity, and surveillance remained separate control domains inside one proposition.

### Permission to scale a merchant relationship

[Payment-terminal hardware as a service](./projects/payment-terminal-haas-merchant-growth.md) reframed a ¥38,280 tax-inclusive terminal from a device sale into a merchant lifecycle. The journey—from application through first transaction, qualified use, retention, and expansion—gave Operations, Risk, Payments, and Growth shared states. Time to active fell from fourteen days to roughly 48 hours; 30-day activation reached 72%; six-month activity reached 81%; and subscriber payment volume was 40% higher than the one-time-buyer cohort. The 14-month payback and 3.2× LTV remained modeled rather than passed off as observed six-month value.

### Permission to operate across jurisdictions

[The regulated FinTech cloud and sovereign-data platform](./projects/regulated-fintech-cloud-sovereign-data-platform.md) combined two pressures that are often handled separately: urgent workload performance and legal authority over data. I turned workload priority, jurisdiction rules, regional controls, audit evidence, and release approvals into a reusable “release compiler.” A critical query reached 480 milliseconds; a two-hour reporting job fell to ten minutes; ten planned markets launched with no recorded audit findings; and a $5 million at-risk contract expanded to $7 million. Hashing and locality supported the control design, but neither was treated as permission by itself.

### Permission to grow exposure from evidence

[The Southeast Asia neobank](./projects/southeast-asia-neobank-alternative-credit.md) was designed for a market where roughly 70% of target users lacked formal credit histories. Consented telco behavior supported eligibility, a small first limit created an observable repayment path, and later exposure was earned through behavior rather than inferred entitlement. Embedded distribution and eKYC kept CAC below $10 against paid alternatives above $100. Approval rose from below 10% to above 40%, more than 100,000 active users were reported in 90 days, and early NPL was 2.4%, with seasoning limitations preserved.

## Product-strategy answer — real-time risk

**Q: Give an example where you identified a problem, developed the product strategy, and drove a quantified outcome.**

**A:** I identified that our risk problem was not simply slow infrastructure. Trade decisions were being evaluated through fragmented schemas and retrospective controls: checks took about 90 milliseconds, 15% of activity entered manual review, and teams could not cleanly separate a hard policy violation from an unusual but legitimate trade.

My root-cause analysis decomposed the path from order creation through normalization, deterministic limits, anomaly detection, decision, and audit. Production traces and review outcomes ruled out three tempting explanations. More compute alone would not fix inconsistent trade meaning. A more sophisticated anomaly model would not resolve conflicting limits. Adding reviewers would increase capacity but preserve the slow, unexplainable decision path. The structural causes were the lack of a common trade language, rules and suspicion being mixed together, and no safe method for transferring authority to a real-time system.

I set the strategy around four product decisions. First, every venue and asset class had to compile into one governed trade model. Second, deterministic capital, concentration, and eligibility rules remained outside machine-learning judgment. Third, anomaly detection explained why a trade was suspicious and routed only the necessary cases. Fourth, degraded modes and staged promotion ensured the system failed safely and earned authority one gate at a time.

The PRD defined user decisions, latency and risk outcomes, scope, and promotion metrics. Engineering used the RFC to compare stream, rules, feature, and serving architectures. The common-trade representation and authority boundary were captured as hard-to-reverse ADRs. A three-month shadow period and launch-readiness checklist required performance, decision equivalence, reason-code quality, fallback, reconciliation, Risk approval, and Operations ownership before production transfer.

The result was a risk check that moved from 90 milliseconds to 4.2 milliseconds. Shadow comparison reached roughly 98% overall agreement, false positives fell about 90%, and the platform blocked $15 million of harmful exposure. Finance reported $85 million of released internal risk or balance-sheet capacity. I preserve that definition rather than calling it regulatory capital or a simple return on the roughly $10 million build.

I owned the problem definition, causal diagnosis, product boundary, roadmap, cross-functional trade-offs, promotion gates, and executive outcome account. Engineering built the platform, Risk and Compliance retained policy authority, and Trading retained business decisions. The strategy succeeded because it made faster decisions and clearer accountability the same product outcome.

## The portfolio-level product thesis

These products span agents, payments, credit, trading, risk, custody, cloud, and merchant services, but they share one architecture:

**identify the actor → define the permitted state → make the decision → execute atomically → preserve evidence → learn without silently expanding authority**

I own the product choices that make that architecture useful: customer and workflow definition, roadmap priority, policy boundaries, real-time decision design, partner and platform interfaces, launch gates, cohort economics, and the evidence used to expand. Trust becomes a growth mechanism when the safe path is also the fastest understandable path.
