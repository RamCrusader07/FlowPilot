---
name: implement
description: "Implement code changes for a Jira ticket with dependency-aware execution. Use when: writing code, making changes, fixing bugs, implementing features, updating configurations, coordinating cross-repo changes with approval gates."
argument-hint: "Jira issue key or plan/design output"
---

# Implement

Implement the changes described by a Jira ticket, handling local and cross-repo dependencies with explicit approval gates.

## When to Use

- Ready to write or modify code for a ticket
- Bug fix, feature implementation, or config change
- Cross-repo changes need coordinated implementation
- After analysis/plan/design phases are complete

## Procedure

1. Review the ticket and identify implementation scope
2. Assess dependencies — classify as local, external-no-change, or external-change-required
3. Request user approval before modifying any external repository
4. Implement the smallest complete change satisfying the ticket
5. Run tests, build, lint, and type-check to validate
6. Report changed files, validation results, and remaining blockers

Full agent instructions: [implement.md](../../../implement/implement.md)
