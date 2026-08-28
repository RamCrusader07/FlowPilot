---
name: orchestrator
description: "Orchestrate the full FlowPilot pipeline for a Jira ticket. Use when: running the complete workflow, delegating to agents, selecting which flows to execute, choosing LLM models by complexity, generating repo instructions. Handles ticket routing, flow selection, and model assignment."
argument-hint: "Jira issue key (e.g. OC-74)"
---

# Orchestrator

Coordinate the FlowPilot pipeline: generate repo instructions, route tickets through the right flows, and select LLM models by complexity.

## When to Use

- Starting a full pipeline run for a Jira ticket
- Need to determine which agents a ticket should flow through
- Want to optimize model selection based on task complexity
- First-time setup of a repo's `instructions.md`

## Procedure

1. **Fetch** the ticket via the fetch skill
2. **Generate repo instructions** — scan the target repo for coding standards, patterns, dependencies, and architecture; write `instructions.md` if missing
3. **Classify the ticket** — determine category (feature, bug, docs, spike, hotfix, etc.) and select the appropriate agent flow
4. **Assess complexity** — score scope, ambiguity, risk, and novelty to assign a model tier (fast/balanced/capable) per agent
5. **Execute the selected flow** with assigned models
6. **Return the review output** to the user

## Flow Routing Summary

| Category | Flow |
|----------|------|
| Feature / UI | fetch → analyse → plan → design → implement → test → review |
| Bug fix | fetch → analyse → plan → implement → test → review |
| Documentation | fetch → analyse → implement → review |
| Investigation / Spike | fetch → analyse → review |
| Hotfix / P0 | fetch → analyse → implement → test → review |

Full agent instructions: [orchestrator.md](../../../workflow/orchestrator.md)
