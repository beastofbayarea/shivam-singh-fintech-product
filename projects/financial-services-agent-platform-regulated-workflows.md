# Giving a Financial-Services Agent Permission to Act

I led a product for financial institutions that needed software agents to do real work safely. I had identified that teams could make convincing demonstrations but could not let the software read private records or act in a live process with clear limits and accountability. I worked with bank and insurer product teams, risk and compliance leaders, developers, platform and security teams, operations owners, sales teams, and end users.

The work sits in my AWS role beginning in July 2024. Compliance review could add six to eight weeks when a team could not reconstruct what an agent had read, decided, called, or changed. The product brief therefore began at the point where the demo stopped.

I owned the product contract that let institutions move from prototypes to governed work: the managed first mile, private-knowledge path, action tiers, identity context, trace profiles, runaway-work brakes, model routing, and workflow approval standard. That joined customer adoption and unit economics in one platform decision, including a reported $12 million annualized routing case and more than 250,000 annualized support hours—both preserved as modeled run rates, not booked savings.

## Six production blockers became one execution contract

| Pilot stopped because… | Platform promise | Release evidence |
|---|---|---|
| orchestration was custom and brittle | managed plan–act–validate loop | successful and failed path tests |
| private knowledge required separate infrastructure | integrated managed retrieval | source, citation, freshness, and access result |
| the agent's authority was unclear | permissioned action groups | authenticated principal, scoped action, parameters |
| reviewers could not reconstruct behavior | configurable execution trace | versioned model, sources, tool calls, approvals, outcome |
| a failed tool could create an endless loop | iteration, time, and spend circuit breakers | limit breach and safe-stop test |
| every request used the premium model | quality- and risk-aware routing | task class, selected model, quality, latency, unit cost |

This was the product: not a more fluent answer, but a contract for who could invoke which workflow, over which data, through which actions, with what stop conditions and evidence.

## I chose a managed first mile

Advanced customers wanted to bring their own vector database and orchestration. Most teams, however, were spending the majority of their initial effort assembling undifferentiated retrieval plumbing before testing a financial workflow.

I made managed knowledge retrieval the default and left extension points for custom stores. The default path could create a grounded knowledge base in under five minutes rather than days. AWS documentation confirms that Bedrock Knowledge Bases can return citations to retrieved source chunks; it also warns that ACL-aware filtering is not authentication. The application still has to authenticate the user and provide trustworthy identity context.

That distinction shaped the product boundary:

`authenticate person/service → authorize data and action → retrieve allowed evidence → plan bounded action → confirm if required → execute → record outcome`

A network location or a matching metadata field never implied trust by itself. NIST Zero Trust Architecture supplied that resource-by-resource principle.

## Actions were grouped by consequence

I used four risk tiers instead of attaching the same control burden to every task.

**Read:** retrieve and summarize approved information. No external state change; citations and access evidence required.

**Draft:** prepare a document, case note, or recommendation. Output stayed uncommitted and carried source and model metadata.

**Reversible action:** update a case, schedule a task, or submit a recoverable workflow step. Required action schema, idempotency key, permissions, and compensating action.

**High-consequence action:** move money, alter a binding record, approve a regulated document, or create material customer impact. Required explicit human confirmation or return of control to the host application.

Amazon Bedrock Agents supports both patterns: a developer can request user confirmation before a function is called, or configure an action group to return the proposed function and parameters to the application. I used those primitives to keep approval in the institution's workflow rather than asking the model to decide whether it should supervise itself.

## Trace depth was a product decision, not a binary switch

Full tracing added about 200 milliseconds per call in the retained tests and increased storage and data-governance cost. No tracing made testing, review, and incident response impossible.

I specified trace profiles by environment and consequence:

- development retained detailed orchestration and tool evidence for diagnosis;
- routine production retained critical decision, source, action, error, and outcome events;
- high-consequence actions retained the full approval package;
- sensitive values were minimized or redacted rather than copied into every trace.

AWS's trace interface exposes orchestration steps, knowledge-base lookups, action inputs and outputs, and failure reasons. That technical capability still needs retention, access, redaction, and review policy; “trace enabled” is not equivalent to an audit program.

## Runaway work had three brakes

An agent could fail through repetition even when every individual call was permitted. I introduced limits on iterations, wall-clock time, and spend. Tool errors were classified as retryable, non-retryable, or human-required. Repeated failure opened the circuit and returned the last safe state with evidence.

The cost path classified task complexity and consequence before selecting a model. Routine work could use a smaller model; difficult or high-stakes work used advanced reasoning. The routing decision was logged so a lower bill could not conceal a quality drop.

AWS launched Intelligent Prompt Routing in preview in December 2024 and later made it generally available; the product page reports up to 30% cost reduction for supported same-family routing. The internal record reports as much as 50% on routine traffic, so I present that as a measured portfolio result rather than an AWS-wide product claim.

## The results belong to different denominators

| Measure | Baseline | Result | How it was measured | Interpretation |
|---|---:|---:|---|---|
| portfolio deployment time | existing pilot cohort | 40% faster | median prototype-to-pilot deployment tickets | broad portfolio result |
| selected blocked pilots | 8 weeks | 3 days | open-to-production-ready milestone | 92.5% reduction for selected cases, not the portfolio median |
| knowledge setup | days | <5 minutes | create-to-first grounded retrieval | initial knowledge path only |
| routine model cost | prior routing mix | up to 50% lower | routed requests × model prices and volumes | maximum for routine class |
| annualized model savings | implied ~$24M baseline if 50% applies to all scope | ~$12M | routing log and billing model | requires confirmation that scopes match |
| legacy modernization effort | manual baseline | nearly 80% less | beachhead workflow estimate | not every legacy program |
| mortgage close likelihood | non-agent users | 3× among agent users | observed cohort | association; selection and workflow differences may contribute |
| support capacity | manual handling | >250,000 hours annualized | handled volume × time difference | modeled annual run rate, not necessarily eliminated headcount |

The two deployment numbers are not contradictory once the cohorts are named: 40% was the broader program change; eight weeks to three days was a lighthouse outcome. The mortgage result is not a randomized causal claim. The support-hours result is capacity value, not automatically payroll savings.

## How I would approve a workflow

Before a production launch, the owner had to show task completion, source accuracy, action validity, unauthorized-action rate, human-intervention rate, error recovery, cost per completed workflow, latency by risk tier, and evidence completeness. A beautiful conversation that never completed an approved task did not count as adoption.

I owned the customer research, production-blocker map, managed-default decision, risk tiers, action and trace policy, cost-routing proposition, beachhead selection, and business measurement. Customer control owners retained approval; application teams authenticated users and defined business permissions; workflow owners approved actions; platform engineering implemented and operated the runtime.

The product's strategic value was simple: governance was not overhead around the agent. It was what allowed an institution to give the agent useful authority.

### Product references

- [Amazon Bedrock Agents — user confirmation](https://docs.aws.amazon.com/bedrock/latest/userguide/agents-userconfirmation.html)
- [Amazon Bedrock Agents — return of control](https://docs.aws.amazon.com/bedrock/latest/userguide/agents-returncontrol.html)
- [Amazon Bedrock Agents — trace events](https://docs.aws.amazon.com/bedrock/latest/userguide/trace-events.html)
- [Amazon Bedrock Intelligent Prompt Routing](https://aws.amazon.com/bedrock/intelligent-prompt-routing/)
- [NIST Generative AI Profile](https://doi.org/10.6028/NIST.AI.600-1) and [NIST Zero Trust Architecture](https://doi.org/10.6028/NIST.SP.800-207)
