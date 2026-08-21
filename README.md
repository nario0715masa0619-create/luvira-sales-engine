# Luvira Sales Engine

Luvira Sales Engine is a documentation-first foundation for a sales execution
engine that helps Luvira validate short-term revenue opportunities with small
and mid-sized businesses.

## Why it exists

**Fact:** Luvira Opportunity Engine is waiting for external API approvals,
including the National Tax Agency Corporate Number Web-API and gBizINFO access.

**Decision:** This separate project explores lawful, API-independent company
discovery and human-reviewed sales preparation while those approvals are
pending.

## How it differs from Opportunity Engine

**Decision:** Opportunity Engine remains focused on evidence-driven, high-value
AI/DX opportunity discovery. Sales Engine focuses on short-term sales execution:
finding candidates, preparing materials, recording outcomes, and learning which
segments convert. The systems must remain separate; any future integration uses
a formal evidence boundary.

## MVP goal

**Hypothesis:** Company-specific website samples and sales materials can earn
replies, meetings, and orders from companies with no official website or a
clearly weak web presence.

The MVP is documentation and an experiment design only. It does not include
application code, scrapers, Google Maps scraping, automated outreach, or API
assumptions.

## First target hypothesis

**Hypothesis:** Equipment work and specialist construction businesses in a
limited Kansai-area market are a suitable initial segment because public,
API-independent candidate sources may be available and web presence may affect
trust and inquiries.

## First 100-company experiment

**Hypothesis:** The first experiment will collect 70–80 No Website Candidates
and 20–30 Weak Website Candidates, human-review them, prepare at least 50 sales
material sets, and conduct a manual or semi-manual first outreach batch.

See [MVP experiment](docs/product/MVP_EXPERIMENT.md).
The practical first-cohort design is in
[First 100-Company Experiment](docs/product/FIRST_100_COMPANY_EXPERIMENT.md).
Use the header-only manual working template in
[`data/templates`](data/templates/README.md); do not commit real candidate data
without intentional approval.

## Safety and data-source principles

- **Decision:** Discover names from permitted non-website sources first; only
  then research official web presence.
- **Decision:** Evaluate each source for legality, terms, commercial reuse,
  storage permission, reliability, provenance, effort, and automation risk.
- **Decision:** Treat AI output as a draft, never as a verified company fact.
- **Decision:** Require human review before every outreach action.

## Current status

**Fact:** This repository contains the initial product, policy, taxonomy, and
workflow documentation only. Product definition acceptance is required before
implementation begins.
