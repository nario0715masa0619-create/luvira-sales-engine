# First 100-Company Candidate Schema

**Decision:** Use a CSV-compatible record. All fields are optional unless marked
**Required**; blank means unknown, not inferred. Controlled values below keep
the sheet usable for manual work.

## Fields

| Field | Requirement | Notes |
| --- | --- | --- |
| candidate_id | Required | Stable ID |
| company_name, normalized_company_name | Required | Source name; normalized comparison name |
| location_prefecture, location_city | Optional | Publicly observed |
| business_category, subsegment | Required | Reviewed category; initial allocation group |
| discovery_source_name, discovery_source_url, discovery_source_type, discovery_date | Required | Provenance minimum |
| source_terms_checked, source_terms_notes, provenance_notes | Required | `Yes`/`No`/`Unknown`; reviewer context |
| website_status, website_search_queries, official_website_url, website_evidence_notes | Required | Search evidence and conclusion |
| weak_website_signals, no_website_confidence, sales_signals | Optional | Observed values only |
| proposed_offer_tier, proposed_offer_notes | Optional | Offer hypothesis, not outcome claim |
| sample_site_concept_status, sample_site_concept_notes | Required | Draft/review state |
| outreach_message_status, outreach_channel, contact_permission_status | Required | Never implies approval to send |
| human_review_status, human_review_notes, candidate_status | Required | Lifecycle and review decision |
| contact_attempt_count, contacted_at, last_contacted_at, next_follow_up_at, contact_history_note | Optional | Fill after approved manual action |
| reply_status, meeting_status, deal_status | Optional | Fill after approved manual action |
| lost_reason, closed_reason, next_action, owner, notes | Optional | Facts, assumptions, and questions labeled |

## Controlled vocabulary

| Field | Allowed values |
| --- | --- |
| discovery_source_type | Association, Cooperative, Chamber, Local Government, Permit/License List, Manual Seed, Referral, NTA CSV, Other Approved |
| website_status | No Website Candidate, Weak Website Candidate, Has Adequate Website, Not Enough Evidence, Needs Human Review |
| weak_website_signals | Broken Navigation, No Usable Inquiry Route, Obsolete Content, Mobile-Unusable, SNS/Portal Only, Other Observed |
| no_website_confidence | Low, Medium, High |
| sales_signals | No Official Website Found, Weak Website Observed, Inquiry Flow Unclear, SNS/Portal Only, Public Contact Route, Contact Prohibited |
| proposed_offer_tier | 1-Page, Basic Website, Inquiry Flow, Later Upsell, Needs Review |
| sample_site_concept_status | Not Started, Draft, In Review, Approved, Rework, Not Applicable |
| outreach_message_status | Not Started, Draft, In Review, Approved, Sent Manually, Hold, Not Applicable |
| outreach_channel | Email, Contact Form, Phone, Referral, Other Approved, None |
| contact_permission_status | Not Checked, Permitted, Prohibited, Needs Review |
| human_review_status | Not Reviewed, Approved, Rework Required, Rejected, Hold |
| reply_status | Not Contacted, No Response, Replied, Opted Out |
| meeting_status | Not Applicable, Proposed, Scheduled, Completed, Declined |
| deal_status | Not Started, Open, Won, Lost |
| lost_reason | See [Loss Reason Taxonomy](../sales/LOSS_REASON_TAXONOMY.md) |
| closed_reason | Won, Lost, Rejected, Duplicate, Contact Prohibited, Archived Other |

**Decision:** `candidate_status` must use the values and transitions in
[Candidate Status Lifecycle](CANDIDATE_STATUS_LIFECYCLE.md). Multi-value signal
fields use a consistent delimiter selected by the experiment owner.

The header-only working template is at
[`data/templates/first_100_candidates_template.csv`](../../data/templates/first_100_candidates_template.csv).
