# First-100 Candidate Sheet Template

`first_100_candidates_template.csv` is a header-only CSV for a manually
maintained experiment run. Copy it locally as `first_100_candidates_working.csv`
and keep the working data out of Git unless committing it is intentionally
approved.

Use the controlled values and field guidance in
[First 100-Company Candidate Schema](../../docs/data/FIRST_100_CANDIDATE_SCHEMA.md).
For every record, retain source URLs/references, access dates, terms-review
notes, website-search queries, and human-review notes. Unknown facts stay blank;
do not let AI-generated guesses become company facts.

The template contains no companies or personal data. Do not add secrets or
machine-specific paths.

`source_review_template.csv` is a separate header-only record for evaluating a
candidate source before collection. Copy it locally as
`source_review_working.csv`. Do not commit real source-review records unless
that is intentionally approved. Follow the
[Source Review Workflow](../../docs/data/SOURCE_REVIEW_WORKFLOW.md); a source
is not usable for first-100 collection until a reviewer approves it.
