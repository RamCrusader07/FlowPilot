---
name: analyse
description: "Analyse a Jira ticket to produce implementation-ready analysis with dependency mapping. Use when: breaking down a ticket, identifying cross-repo dependencies, understanding change scope, preparing for planning or implementation."
argument-hint: "Jira issue key or ticket data from fetch"
---

# Analyse

Turn fetched Jira ticket details into an implementation-ready analysis with an explicit list of required changes across repositories.

## When to Use

- After fetching a ticket, before planning or implementation
- User needs to understand the scope and dependencies of a ticket
- Cross-repo impact assessment is needed
- Identifying unknowns and blockers before implementation

## Procedure

1. Read the ticket key, description, acceptance criteria, links, and labels
2. Identify current-repository changes needed
3. Inspect integration boundaries, API contracts, and shared-library usage for dependent repos
4. Classify each dependency (local, external no-change, external change-required)
5. Produce a structured dependency assessment

Full agent instructions: [analyse.md](../../../analyse/analyse.md)
