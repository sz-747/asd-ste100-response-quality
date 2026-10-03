# Response Quality Review Prompt

Review the assistant response or transcript with the Response Quality Review Skill.

First identify:

- the user's goal;
- the response's claimed outcome;
- the evidence available;
- the response type.

Select only the applicable modules:

- ASD-STE100 linguistic review;
- response structure review;
- evidence and completeness review;
- terminology review;
- minimalism review.

Return:

- Verdict: clear, usable with minor changes, or confusing/incomplete.
- What worked.
- Issues with module and severity.
- The smallest improvement.
- The expected effect on confusion, rework, and follow-up turns.

Do not force a style rewrite. Do not remove necessary facts. Preserve code, commands, URLs, identifiers, quotations, and error text.
