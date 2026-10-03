# Response Quality Review Skill

A reusable quality-review methodology for assistant responses and interactive transcripts.

It uses ASD-STE100 for linguistic ambiguity, but it also checks response structure, evidence, completeness, terminology, cognitive load, risk, and recovery.

## What this skill is used for

Use this skill to review an assistant response before sending it or to audit an interactive transcript after a conversation. It helps identify why an answer was unclear, incomplete, misleading, inefficient, or harder to act on than necessary.

It checks whether the response:

- answers the user's actual goal;
- states the result, blocker, or next action clearly;
- separates verified facts from inferences and recommendations;
- uses the right response structure for the task;
- gives enough detail without unnecessary explanation;
- uses precise and consistent terminology;
- includes important prerequisites, limits, risks, and recovery steps;
- avoids avoidable follow-up questions and rework.

It is useful for:

- reviewing one draft response;
- reviewing a multi-turn assistant conversation;
- improving agent prompts and skills;
- auditing status reports, plans, explanations, procedures, and handoffs;
- finding recurring response failures worth adding to durable agent instructions.

It is a review methodology, not an AI detector and not a requirement to rewrite every response in strict ASD-STE100 language.

## Scope

This skill reviews output. It does not force every response into a fixed writing style.

## Layout

- `SKILL.md` - user-level skill-discovery entrypoint.
- `skills/skill_response_quality.md` - detailed agent-facing playbook.
- `docs/prd.md` - problem and success criteria.
- `docs/rfc.md` - methodology design and module boundaries.
- `docs/test.md` - review test cases.
- `docs/working.md` - change history and lessons.
- `prompts/response_quality_review.md` - optional review prompt.
