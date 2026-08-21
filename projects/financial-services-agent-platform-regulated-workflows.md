# Giving a financial-services agent permission to act

Financial institutions could build impressive agent demos, but production stopped where private data and real actions began. Review could add six to eight weeks because teams could not reconstruct what an agent had read, decided, called, changed, or cost.

Beginning in my July 2024 AWS role, I defined the product contract that closed this gap across bank/insurer teams, Risk/Compliance, developers, Platform/Security, Operations, Sales, and users.

The product was not a more fluent model. It was a governed execution path:

**authenticate → authorize data and action → retrieve permitted evidence → plan bounded work → confirm by consequence → execute → record outcome**

## Six blockers became one platform surface

1. Custom orchestration became a managed plan–act–validate loop with successful and failed path tests.
2. Separate retrieval plumbing became a managed knowledge path with source, freshness, citation, and access results.
3. Ambiguous authority became permissioned action groups tied to authenticated principals and schemas.
4. Opaque behavior became configurable traces of versions, sources, tools, approvals, and outcomes.
5. Runaway retries became iteration, time, and spend circuit breakers.
6. Premium-model overuse became quality- and risk-aware routing with logged economics.

I chose a **managed first mile** because most customer teams were spending their initial effort on undifferentiated retrieval and orchestration. Advanced teams retained extension points for custom stores. The default path created first grounded retrieval in under five minutes rather than days.

AWS documents that Bedrock Knowledge Bases can return citations, while ACL-aware filtering still is not authentication. That distinction defined the boundary: application teams had to supply trustworthy identity context, and every data/action decision remained resource-specific. [NIST Zero Trust Architecture](https://doi.org/10.6028/NIST.SP.800-207) informed that principle.

## Authority scaled by consequence

**Read:** retrieve and summarize approved information; citations and access evidence required.

**Draft:** create a recommendation, note, or document that remained uncommitted and carried source/model metadata.

**Reversible action:** update a case, schedule a task, or take another recoverable step using permissions, a typed schema, an idempotency key, and a compensating action.

**High-consequence action:** move money, alter a binding record, approve regulated content, or materially affect a customer. The agent returned the proposed action to the host application or required explicit human confirmation.

Amazon Bedrock Agents supports [user confirmation](https://docs.aws.amazon.com/bedrock/latest/userguide/agents-userconfirmation.html) and [return of control](https://docs.aws.amazon.com/bedrock/latest/userguide/agents-returncontrol.html). I used those primitives so the institution’s workflow—not the model—owned approval.

## Trace was a tiered product decision

Full tracing added roughly 200 milliseconds per call in retained tests and increased storage/governance cost. No trace made evaluation, review, and incident response impossible.

I defined profiles:

- development retained detailed orchestration and tool evidence;
- routine production retained critical source, decision, action, error, and outcome events;
- high-consequence actions retained the complete approval package;
- sensitive values were minimized or redacted instead of copied everywhere.

The [Bedrock trace interface](https://docs.aws.amazon.com/bedrock/latest/userguide/trace-events.html) exposes orchestration, retrieval, action inputs/outputs, and failures. Retention, entitlement, redaction, and review still had to turn that capability into an audit program.

## A safe agent also needed economic brakes

A permitted call could still loop indefinitely. I introduced caps on iterations, wall-clock time, and spend. Errors were classified as retryable, terminal, or human-required. Repeated failure opened the circuit and returned the last safe state with evidence.

Task complexity and consequence also selected the model. Routine work used lower-cost capacity where quality gates held; high-stakes tasks used advanced reasoning. The routing choice, quality, latency, and cost were logged together so savings could not conceal a performance decline.

The internal record reports up to 50% cost reduction on routine traffic, compared with the public [Intelligent Prompt Routing](https://aws.amazon.com/bedrock/intelligent-prompt-routing/) claim of up to 30% for supported routing. I preserve the internal figure as a scoped result, not an AWS-wide claim.

## Product and business account

| Workflow question | Baseline → target → recorded result | Measurement |
|---|---|---|
| Could the portfolio move pilots faster? | existing cohort → materially faster → 40% faster | Median prototype-to-pilot milestones across comparable deployment tickets |
| Could lighthouse blockers collapse? | 8 weeks → days → 3 days | Selected open-to-production-ready milestone; 92.5% lower, not portfolio median |
| Could knowledge setup become self-serve? | days → minutes → <5 minutes | Create knowledge base to first grounded retrieval |
| Could routine inference cost fall safely? | routing cost index 100 → lower with quality parity → as low as 50 | Completed routine workflows, model price, quality, latency; maximum scoped result |
| What value did routing model? | implied scope baseline ~$24M if directly comparable → reduce → ~$12M annualized savings | Routing logs × volume/prices; modeled run rate, not booked savings |
| Could a legacy beachhead shrink effort? | manual baseline → large reduction → nearly 80% less | Selected modernization estimate, not every legacy program |
| Did agent use correlate with mortgage progress? | non-agent cohort → improve → 3× close likelihood among users | Observational; selection and workflow differences remain |
| What support capacity was modeled? | manual handling → reduce → >250,000 hours annualized | Eligible volume × time difference; capacity, not automatic headcount removal |

Before production, the owner had to show task completion, source accuracy, action validity, unauthorized-action rate, human intervention, recovery, latency and cost by tier, and evidence completeness. Conversation quality without an approved completed task was not adoption.

Discovery, blocker synthesis, the managed default, consequence tiers, trace/action policy, routing economics, beachheads, release standards, and measurement were my product decisions. Customers approved controls; applications authenticated users and defined permissions; workflow owners approved actions; Engineering ran the platform.

Governance was not overhead around the agent. It was the product capability that let an institution grant useful authority at all.
