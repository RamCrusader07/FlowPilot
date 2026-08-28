---
name: test
description: "Validate implemented changes and produce structured test evidence. Use when: running tests, verifying implementation, checking build status, producing test evidence for CI diagnosis and review."
argument-hint: "Implementation output or changed file paths"
---

# Test

Validate implemented changes and produce a structured evidence bundle for CI Diagnosis and Review agents.

## When to Use

- After implementation is complete
- Need to verify changes pass tests, type checks, and builds
- Producing evidence for the review quality gate
- CI failures need structured artifact collection

## Procedure

1. Select the narrowest tests that validate the implemented behavior
2. Execute tests, type checks, and build checks
3. Capture raw outputs for passed and failed checks
4. Normalize failures with test name, file, line, and error signature
5. Prepare structured evidence bundle for CI Diagnosis and Review handoff

Full agent instructions: [test.md](../../../test/test.md)
