# Candidate Status Lifecycle

**Decision:** `candidate_status` uses the following small controlled lifecycle.
An owner may record discovery and research; a named human reviewer is required
for approval, rejection, contact, and outcome transitions.

| Status | Meaning | May move to | Review required | Terminal |
| --- | --- | --- | --- | --- |
| Discovered | Name captured from a permitted source | Researching, Archived | No | No |
| Researching | Source, identity, and website research in progress | Needs Human Review, Approved For Materials, Rejected | Yes for approval/rejection | No |
| Needs Human Review | Evidence or suitability is unresolved | Researching, Approved For Materials, Rejected, Archived | Yes | No |
| Approved For Materials | Reviewer permits fact-grounded preparation | Materials Ready, Rejected, Archived | Yes | No |
| Rejected | Not suitable, duplicate, prohibited, or insufficient | Archived | Yes | No |
| Materials Ready | Sample and message drafts are ready for review | Approved For Outreach, Needs Human Review, Rejected | Yes | No |
| Approved For Outreach | Reviewer approved materials and permitted channel | Contacted, Archived | Yes | No |
| Contacted | Human sent a reviewed message manually | Replied, Lost, Archived | Human records | No |
| Replied | A response was received | Meeting Scheduled, Won, Lost, Archived | Human records | No |
| Meeting Scheduled | A meeting is arranged | Won, Lost, Archived | Human records | No |
| Won | Paid order confirmed | Archived | Human records | Commercial terminal |
| Lost | Sales attempt closed without order | Archived | Human records | Commercial terminal |
| Archived | Record retained with a closed reason | — | Human records | Administrative terminal |

**Decision:** `Won` and `Lost` are commercial terminal statuses: no further
active sales progression is expected, but either may move once to `Archived` for
administrative closure. `Archived` is the administrative terminal status and
must not normally return to an active workflow unless a future approved process
explicitly reopens it.

## Outreach gate

**Decision:** Only a human reviewer may set `Approved For Outreach`, after
confirming plausible identity, recorded provenance, documented website search,
permitted contact route, no contact prohibition, appropriate offer, and that
sample/message contain no invented or misleading company facts.

**Decision:** A reviewer may return any non-terminal record to `Researching` or
`Needs Human Review` when evidence changes. Never bypass review by moving from
`Discovered` directly to `Contacted`.

Follow-up limits and recording fields are defined in
[First 100-Company Experiment](../product/FIRST_100_COMPANY_EXPERIMENT.md).
