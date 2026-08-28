---
name: ci-diagnosis
description: "Diagnose CI failures using read-only evidence analysis. Use when: CI pipeline fails, investigating test failures, clustering related failures, determining root cause of build or test breakage, producing diagnosis reports."
argument-hint: "CI run ID, commit SHA, or test evidence bundle"
---

# CI Diagnosis

Investigate CI failures using read-only evidence and produce a structured, citation-backed diagnosis report.

## When to Use

- CI pipeline has failed and root cause is unclear
- Test failures need clustering and deduplication
- Need to distinguish product defects from environment instability
- Producing a diagnosis report for the review quality gate

## Procedure

1. Ingest evidence: run ID, commit SHA, failure summaries, logs, and artifacts
2. Normalize failures into consistent fields (test name, file, line, error signature)
3. Cluster related failures by deterministic signals (file overlap, shared error signatures)
4. Assign confidence levels and classify outcomes
5. Produce a schema-versioned diagnosis report with per-cluster rationale and next-best actions

Full agent instructions: [ci-diagnosis.md](../../../ci-diagnosis/ci-diagnosis.md)
