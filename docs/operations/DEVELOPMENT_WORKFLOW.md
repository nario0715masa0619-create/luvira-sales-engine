# Development Workflow

## Before changes

**Decision:** Inspect repository state, branch, remote URL, and working tree. If
the state is unexpectedly dirty or the repository is unexpected, stop and report.

## During changes

**Decision:** Keep documentation concise; preserve Fact, Hypothesis, Decision,
and Open Question labels. Do not begin implementation until the product
definition is accepted.

## Before reporting

**Decision:** List changed files; run applicable formatting/checks, `git diff
--check`, secret scanning, and machine-specific absolute-path scanning. Commit
once only if all checks pass. Never push without explicit instruction.
