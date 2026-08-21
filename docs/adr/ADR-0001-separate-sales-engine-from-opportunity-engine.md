# ADR-0001: Separate Sales Engine from Opportunity Engine

## Status

Accepted.

## Decision

Luvira Sales Engine is a separate repository and product boundary. Future
integration, if any, uses a formal evidence contract.

## Rationale

Opportunity Engine optimizes evidence-driven, high-value opportunity discovery;
Sales Engine validates short-term execution. Combining them would import
unneeded architecture and contaminate evidence models with sales intuition.
