---
name: skill-quality-review
description: "Evaluate a reusable skill on representative cases and record observed failures before revising the instructions."
---

# Skill Quality Review

## Inputs
Skill version, intended task, representative cases, available tools, quality rubric, and comparison version where relevant. Keep case-specific answers out of the instructions being evaluated.

## Workflow
Define expected behavior before running cases. Include a normal request, missing data, and a changed-direction or conflicting-input case. For analysis, include zero denominators or overlapping conversions. Run only within task permissions and save actual inputs/outputs.

Score preserved intent, factual grounding, useful output, uncertainty, and authorization boundaries. Record time and human rework only if measured. Compare versions on the same cases, then make the smallest useful change and retest.

## Output and checks
Return case results, failures, limitations, and proposed revisions. Distinguish metadata validation from behavioral testing and live business validation. Do not report an unrun test as passed or generalize reliability from a few easy cases.
