# Source Review Workflow

**Decision:** A source review record evaluates one proposed source before any
candidate collection. It is separate from candidate records and does not itself
approve a source.

## Controlled vocabulary

| Field | Allowed values |
| --- | --- |
| source_type | Industry Association, Cooperative, Chamber Of Commerce, Local Government Directory, Permit License List, Public Business Directory, Manual Seed List, Referral List, Other |
| public_access_status | Public, Public With Restrictions, Login Required, Unknown |
| login_required | Yes, No, Unknown |
| terms_checked | Yes, No, Not Found, Needs Review |
| commercial_use_status | Allowed, Not Prohibited, Prohibited, Unclear, Needs Human Decision |
| storage_reuse_status | Allowed, Not Prohibited, Prohibited, Unclear, Needs Human Decision |
| manual_collection_allowed_status | Allowed, Not Prohibited, Prohibited, Unclear, Needs Human Decision |
| automation_allowed_status | Allowed, Prohibited, Unclear, Not Needed For MVP |
| provenance_quality | High, Medium, Low, Unknown |
| estimated_candidate_density | High, Medium, Low, Unknown |
| approval_status | Proposed, Terms Review Needed, Approved For Manual Collection, Rejected, Needs Legal / Human Decision |
| approved_collection_method | Manual Copy, Manual Research, Manual Verification Only, Not Approved, Future Review Required |

## Approval rule

**Decision:** A human reviewer may set `Approved For Manual Collection` only
when public access or access conditions are clearly acceptable; terms have been
checked or reasonably searched and not found; commercial use, storage/reuse, and
manual collection are allowed or not prohibited (or explicitly approved by a
human decision); provenance can be recorded; and the intended activity needs no
prohibited scraping or Google Maps data extraction. The source must not prohibit
sales, reuse, storage, or commercial contact in a way that affects planned use.

## Rejection rule

**Decision:** Reject a source if it prohibits relevant commercial use, storage,
or reuse; requires login with unclear terms; is Google Maps scraping or depends
on extraction outside allowed API terms; has unclear provenance; is a purchased
list without clear provenance/rights; or creates unacceptable legal or
reputational risk.

## Process

1. Create a `Proposed` row in the header-only working copy.
2. Record access, terms, intended use, provenance, and candidate-density notes.
3. Route uncertainty to `Terms Review Needed` or `Needs Legal / Human Decision`.
4. A human reviewer sets `Approved For Manual Collection` or `Rejected`.
5. Only then may manual candidate collection begin.

Use [First Source Selection](FIRST_SOURCE_SELECTION.md) for priority order and
the [source-review template](../../data/templates/source_review_template.csv)
for the record fields.
