# Response Quality Review Skill

## Layout

- `SKILL.md` is the user-level discovery entrypoint.
- `skills/skill_response_quality.md` is the public review playbook.
- `docs/` contains the problem definition, design, tests, and working log.
- `prompts/` contains optional invocation prompts.

## Operating rules

1. Review the response against the user's task and evidence.
2. Select only the applicable review modules.
3. Treat ASD-STE100 as one linguistic module, not the complete methodology.
4. Do not remove necessary facts to make text shorter.
5. Preserve code, commands, URLs, identifiers, quotations, and error text.
6. Report the smallest useful improvement.
7. Do not claim formal ASD-STE100 compliance from a heuristic review.
