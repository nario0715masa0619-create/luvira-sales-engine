# Public Source Review Plan

## Why this is next

**Fact:** Earlier association/cooperative directories were useful but remain
`Needs Legal / Human Decision` because permission for commercial reuse, storage,
or outreach was unclear.

**Decision:** Review public/government-like sources next. Their publication
purpose and conditions may be clearer, but public availability never by itself
approves collection or outreach.

## Priority

**Hypothesis:** Prioritize Hyogo, Osaka, then Kyoto; expand to Nara, Shiga,
Wakayama, and Okayama only if reviewed supply is insufficient. Start with
electrical, HVAC, and plumbing/pipework; use fire equipment, communications, or
building maintenance only as fallback subsegments.

## Source categories

| Category | Usefulness and likely fields | Risks and review outcome |
| --- | --- | --- |
| Construction license/permit search or list | Licensed business name, location, license type/category; direct fit for construction subsegments | Confirm publication purpose, terms, reuse, and personal-data exposure. Approve only if manual internal use is not prohibited; escalate uncertainty. |
| Government bidding/supplier qualification list | Supplier name, category, region, qualification period; may identify active local firms | May include procurement-only purpose, contact persons, or reuse limits. Reject explicit prohibitions; escalate unclear conditions. |
| Local-government public business directory | Local name, location, industry/category, public profile | Directory may be promotional but may restrict reuse. Check terms and sales-contact restrictions. |
| Public industrial-promotion/SME support directory | Participating company, specialty, region, public profile | May be programme-specific or stale. Check scope, density, and reuse terms. |
| Chamber/commercial association directory | Local business and category coverage | Review only when terms are clear; otherwise treat as `Needs Legal / Human Decision`. |

## Minimum review checklist

For each concrete URL, record the operator, publication purpose, terms,
copyright/reuse notice, privacy policy where personal data appears, whether data
is business-only or includes personal data, commercial-use status,
storage/reuse status, manual-collection status, sales-contact restrictions,
provenance, and candidate density.

## Approval guidance

**Decision:** A human reviewer may set `Approved For Manual Collection` only
when no relevant prohibition is found; use is limited, manual, and internal;
provenance is recorded; automation is unnecessary; personal-data risk is
acceptable or avoidable; and the reviewer approves. Use `Needs Legal / Human
Decision` for uncertainty and `Rejected` for a relevant prohibition.

## Local working process

**Decision:** Record real URLs only in the ignored local file
`data/local/source_review_working.csv`. Do not commit those URLs. Do not collect
candidate companies until at least one source is approved. See
[Source Review Workflow](SOURCE_REVIEW_WORKFLOW.md) and
[First Source Selection](FIRST_SOURCE_SELECTION.md).
