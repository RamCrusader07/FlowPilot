---
name: review
description: "Final quality and risk assessment before release. Use when: reviewing changes for release readiness, assessing implementation quality, evaluating test evidence and CI diagnosis, determining go/no-go for deployment."
argument-hint: "Implementation and test outputs"
---

# Review

Produce a final quality and risk assessment using implementation results, test evidence, and CI Diagnosis findings.

## When to Use

- After implementation and testing are complete
- Final quality gate before release or PR merge
- Need to assess change readiness with structured findings
- Evaluating risk and residual issues

## Procedure

1. Confirm implemented behavior matches planned scope
2. Evaluate failing/passing checks, diagnosis confidence, and unknowns
3. Report findings ordered by severity with file references and evidence
4. Determine release readiness: ready, conditional, or blocked
5. Provide explicit follow-up actions for each blocker

Full agent instructions: [review.md](../../../review/review.md)
