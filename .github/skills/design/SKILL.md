---
name: design
description: "Produce a technical design for implementation. Use when: designing new components, defining API contracts, specifying schemas, planning architecture changes, creating interface specifications, mapping component-level changes."
argument-hint: "Plan output or Jira issue key"
---

# Design

Translate the implementation plan into precise, build-ready technical decisions covering components, interfaces, contracts, and rollout.

## When to Use

- Ticket introduces new components, interfaces, or schemas
- API contract or architecture changes are needed
- Feature or UI work requiring detailed technical specification
- Cross-repo contract design is needed

## Procedure

1. Define design scope — in-scope vs out-of-scope components
2. Map current and target behavior against acceptance criteria
3. Specify interface and contract changes (endpoints, events, schemas, config)
4. Design component-level changes with responsibilities, I/O, control flow, and failure handling
5. Define observability, test strategy, and rollout plan

Full agent instructions: [design.md](../../../design/design.md)
