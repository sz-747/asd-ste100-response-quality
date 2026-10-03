---
name: response-quality-review
description: Review assistant responses and transcripts for task fit, evidence, structure, clarity, completeness, terminology, risk, and user effort.
user-invocable: true
---

# Response Quality Review

This is the public agent-facing playbook. Use it after drafting a response or when auditing a transcript.

## Required sequence

1. State the user's goal in one sentence.
2. State the response's outcome in one sentence.
3. List claims that require evidence.
4. Classify the response type:
   - Tutorial: teaches a skill.
   - How-to: helps complete a task.
   - Reference: describes facts or options.
   - Explanation: clarifies why or how something works.
   - Conversation reply: answers or advances an interactive decision.
5. Select the applicable review modules.
6. Find the highest-impact issue.
7. Recommend the smallest correction.

## Review modules

### ASD-STE100 linguistic review

Check for ambiguous wording, overloaded sentences, passive procedures, inconsistent terms, undefined abbreviations, vague references, and hidden conditions.

Use the standard as a quality lens. Do not force its controlled vocabulary or sentence limits when technical accuracy or conversational clarity would suffer.

### Response structure review

Use:

- **BLUF:** Put the answer, outcome, blocker, recommendation, or requested action first.
- **Diátaxis:** Do not mix tutorial, how-to, reference, and explanation content without a clear reason.
- **Information Mapping:** Give each information unit one purpose, a clear label, and a predictable structure.
- **Progressive disclosure:** Put the immediate path first. Move secondary detail behind clear labels or an offer to continue.

### Evidence and completeness review

Check whether the response distinguishes:

- Checked facts.
- Changes actually made.
- Inferences.
- Recommendations.
- Pending work.
- Unverified claims.

Keep information that prevents misunderstanding, wrong actions, missed prerequisites, or predictable follow-up questions. Remove repetition and decorative detail first.

### Terminology review

Use one term for one concept. Define unfamiliar terms. Flag synonym drift. Preserve exact product names, commands, paths, URLs, identifiers, and error text.

### Minimalism review

Start from the user's real task. Give a useful early action. Keep explanation near the task. Include checkpoints and recovery for predictable errors.

## Output format

```text
Verdict: clear | usable with minor changes | confusing/incomplete

What worked:
- ...

Issues:
- [module] [severity] Finding. Evidence: "..."

Smallest improvement:
- ...

Conversation effect:
- ...
```

For transcript reviews, add:

- repeated pattern
- affected turns
- applicable module
- expected reduction in confusion, rework, or follow-up turns

## Quality questions

- What is the user trying to decide or do?
- What would the user misunderstand?
- What would the user need to ask next?
- Which claim is least supported?
- Which detail prevents an operational mistake?
- Which single change gives the largest improvement?
