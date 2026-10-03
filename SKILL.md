---
name: asd-ste100-response-quality
description: Review assistant responses and interactive conversations for clarity, structure, evidence, completeness, and user effort. Uses ASD-STE100 as one linguistic check, not as the whole writing method.
user-invocable: true
metadata:
  type: QualityMethodology
  scope: user-level
---

# Response Quality Review Skill

Use this skill to evaluate a response or conversation. Do not automatically rewrite the response in a fixed style.

The canonical project-style guide is in `skills/skill_response_quality.md`. The supporting design and test documents are in `docs/`.

## Review workflow

1. Identify the user's goal, decision, or requested outcome.
2. Identify the response's claimed outcome.
3. Check the claim against the available evidence.
4. Classify the response as a tutorial, how-to guide, reference, explanation, or conversation reply.
5. Check whether the information is relevant, findable, understandable, and usable.
6. Check language ambiguity with ASD-STE100-inspired rules.
7. Check terminology, completeness, recovery, risk, and unnecessary user effort.
8. Report the smallest change with the largest improvement.

## Review result

Return:

- **Verdict:** clear, usable with minor changes, or confusing/incomplete.
- **What worked:** the strongest evidence of quality.
- **Issues:** each issue with its review dimension.
- **Smallest improvement:** the exact change or replacement pattern.
- **Conversation effect:** the expected reduction in confusion, rework, or follow-up turns.

For a transcript, also report repeated patterns and the response turns where they affected the conversation.

## Method selection

Use only the checks that match the response:

- `asd-ste100`: ambiguity, sentence overload, passive procedures, terminology consistency.
- `response-structure`: BLUF, Diátaxis, Information Mapping, progressive disclosure.
- `evidence-completeness`: factual support, uncertainty, prerequisites, limitations, recovery.
- `terminology`: one term per concept, definitions, naming drift.
- `minimalism`: task-first guidance, useful early action, exploration, and error recovery.

Do not apply every check mechanically. The user's goal and the technical facts have priority.

## Guardrails

- Do not confuse concise with complete.
- Do not delete facts merely to shorten a response.
- Do not treat ASD-STE100-inspired review as formal ASD-STE100 certification.
- Preserve code, commands, URLs, identifiers, quotations, and error text exactly.
- Do not invent evidence, examples, status, or user intent.
