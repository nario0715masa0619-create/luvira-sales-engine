# Candidate Schema

**Decision:** A candidate record is evidence-led and reviewable. Required fields:

| Field | Purpose |
| --- | --- |
| candidate_id | Stable internal identifier |
| company_name | Source-recorded name |
| location | Publicly observed location |
| business_category | Source-recorded or reviewed category |
| discovery_source | Source type and reference |
| provenance | URL/reference, access date, use assessment |
| website_status | Taxonomy value and evidence |
| website_weakness_signals | Observed signals only |
| candidate_status | Workflow status |
| proposed_offer | Reviewable offer hypothesis |
| sample_status | Not started/draft/reviewed/approved |
| outreach_status | Not drafted/reviewed/approved/sent/manual hold |
| human_review | Reviewer, date, decision, note |
| contact_outcome | Not contacted/reply/meeting/won/lost |
| lost_reason | Observed or stated reason |
| notes | Clearly labeled facts, assumptions, and questions |

**Decision:** Unknown values remain unknown; do not infer them.

For the first experiment's CSV-compatible field set and controlled values, see
[First 100-Company Candidate Schema](FIRST_100_CANDIDATE_SCHEMA.md). Candidate
lifecycle values are defined in [Candidate Status Lifecycle](CANDIDATE_STATUS_LIFECYCLE.md).
