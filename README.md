# Response Quality Review Skill

A reusable quality-review methodology for assistant responses and interactive transcripts.

It uses ASD-STE100 for linguistic ambiguity, but it also checks response structure, evidence, completeness, terminology, cognitive load, risk, and recovery.

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
