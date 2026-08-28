# FlowPilot
Repo For SAS Ai hackathon 2026

## Pipeline

FlowPilot stages are organized as a handoff pipeline:

1. Fetch
2. Analyze
3. Plan
4. Design
5. Implement
6. Test
7. CI Diagnosis
8. Review

## Stage Purpose

- `fetch/fetch.md`: Retrieve Jira issues and provide structured ticket data.
- `analyse/analyse.md`: Convert ticket details into implementation-ready analysis and dependency findings.
- `plan/plan.md`: Produce phased execution plans with validation and dependency gates.
- `design/design.md`: Define technical design decisions, contracts, and rollout strategy.
- `implement/implement.md`: Implement approved changes and validate outcomes.
- `test/test.md`: Execute and summarize verification output for downstream diagnosis and review.
- `ci-diagnosis/ci-diagnosis.md`: Diagnose CI failures using evidence-only, read-only investigation.
- `review/review.md`: Perform final quality review with risk-focused findings and release readiness.
