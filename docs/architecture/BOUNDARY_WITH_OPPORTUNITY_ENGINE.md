# Boundary with Opportunity Engine

**Decision:** Luvira Sales Engine is separate from Luvira Opportunity Engine.
It must not adopt Opportunity Engine's canonical architecture, ICP, scoring,
anti-bias controls, HumanReview model, or acceptance-run process.

## Permitted future boundary

**Decision:** A formal future handoff may include `company_identity`,
`provenance`, `public_evidence`, `observed_sales_signal`, `human_review_note`,
and `sales_outcome_summary`.

## Prohibited handoff

**Decision:** Do not pass unsupported guesses, buyer-likelihood intuition,
AI-invented facts, unverified signals, or sales outcomes represented as direct
ICP truth.

## Open Question

What evidence contract and consent/privacy review are needed before integration?
