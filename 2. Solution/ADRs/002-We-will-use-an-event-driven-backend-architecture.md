
---

# Use and event-driven architecture

Date: 2022-11-07

## Status

Confirmed

## Context

[Analysis of the architecture characteristics](../Architecture%20Style%20Analysis/README.md) required of the system and the possible architecture styles concluded that an event-driven architecture would suit the system, with less trade-offs than other options.

## Decision

Use an event-driven architecture for the backend of the system.

## Consequences

**Positive:**

- Four of seven characteristics score highly.

**Negative:**

- Interoperability needs to be mitigated.

**Risks:**

- Interoperability and configurability may still be high trade-offs after mitigation.

---
