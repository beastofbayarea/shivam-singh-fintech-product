# Moving Financial-Services Agents from Demos into Governed Workflows

I led this product work during my [AWS experience beginning in July 2024](https://github.com/beastofbayarea/shivam-singh-fintech-product/blob/main/shivam-singh-fintech-product.pdf).

Financial-services teams could demonstrate that an agent understood a question. They could not reliably put that agent in charge of a regulated workflow. Production stalled on permissions, private-data access, auditability, runaway execution, human approval, and unit economics. In some cases, missing traceability alone added six to eight weeks to compliance review.

I reframed the product from “better conversation” to “governed action.”

## I mapped blockers to platform capabilities

I interviewed application, risk, compliance, and platform teams around the point at which each pilot stopped. That produced a product map with six connected capabilities:

- managed reasoning and orchestration;
- an integrated private knowledge layer;
- permissioned tool actions;
- configurable traces and evidence;
- execution limits, circuit breakers, and human approval; and
- cost-aware model routing.

The NIST Generative AI Profile supplied the primary risk frame. I used its treatment of confabulation, privacy, cybersecurity, transparency, human oversight, and measurement to turn broad concerns into workflow requirements and acceptance criteria.

## Grounding had to be the fastest safe path

Advanced teams wanted maximum retrieval flexibility, but most customers were spending days assembling a basic RAG path before they could test a business workflow. I made managed retrieval the default journey and kept extension points for teams that needed custom orchestration.

That choice reduced knowledge-base setup from days to under five minutes. It also preserved controlled access to private financial data. NIST's Zero Trust Architecture influenced the access design: no user, agent, tool, or data source received implicit trust based on network location. Each resource request had to be evaluated against identity, policy, and least privilege.

## I made control depth proportional to workflow risk

Full tracing can add latency and storage cost. No tracing makes review and incident response impossible. I made trace depth configurable by environment and risk class, then defined the minimum evidence required for each production workflow.

I also classified tasks by complexity and consequence. Routine requests could use a lower-cost model. Complex or high-stakes work used advanced reasoning, tighter execution limits, and explicit human checkpoints. Circuit breakers stopped repeated tool calls or cost escalation before an agent could turn an error into an uncontrolled process.

This architecture let teams trade latency and cost consciously instead of removing controls to meet a performance target.

## I measured completed regulated work

Prototype count was not a useful product metric. I tracked deployment time, time to first grounded workflow, compliance-review delay, task completion, intervention, error behavior, cost per completed workflow, and the operational outcome of each beachhead use case.

The results included:

- a 40% improvement in deployment time, with selected pilots moving from eight weeks to three days;
- knowledge-base setup in under five minutes;
- routine-query cost reductions of as much as 50%, supporting about $12 million in annualized savings;
- nearly 80% less legacy-modernization effort in a beachhead workflow;
- mortgage-agent users becoming three times more likely to close; and
- more than 250,000 support hours saved annually.

## The product principle I retained

In regulated AI, governance is not packaging around the product. Permissioning, traceability, limits, approvals, and recovery are the features that make useful action possible. I design them into the workflow and measure the resulting business outcome—not the number of impressive conversations.

## External foundations

These sources supplied the primary risk and access-control methodology. My resume is linked only to establish employment chronology.

| Source | How I applied it |
|---|---|
| [NIST — Generative AI Profile (2024)](https://doi.org/10.6028/NIST.AI.600-1) | I used its risk taxonomy and measurement guidance to convert production concerns into workflow controls and release evidence. |
| [NIST — Zero Trust Architecture (2020)](https://doi.org/10.6028/NIST.SP.800-207) | I used its per-resource, identity-aware, least-privilege model for agent access to private data and tools. |
