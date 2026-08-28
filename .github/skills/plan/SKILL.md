---
name: plan
description: "Create a phased implementation plan from ticket analysis. Use when: breaking work into execution phases, defining task-level actions, sequencing cross-repo changes, planning validation and rollout."
argument-hint: "Analysis output or Jira issue key"
---

# Plan

Convert analysis into an actionable, phased implementation plan with clear task ownership and dependency gates.

## When to Use

- After analysis is complete, before design or implementation
- Work needs to be broken into ordered phases
- Cross-repo sequencing constraints must be planned
- User needs a clear execution roadmap for a ticket

## Procedure

1. Restate scope and success conditions from analysis
2. Break work into ordered execution phases with clear boundaries
3. Define task-level actions with ownership (current repo, external repo, coordination)
4. Mark tasks requiring user approval for external changes
5. Plan validation checks and rollback steps per phase

Full agent instructions: [plan.md](../../../plan/plan.md)
