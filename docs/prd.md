# Product Requirements: Response Quality Review

## Problem

Assistant output can be fluent but still create confusion. Common failures include wrong response shape, unsupported claims, vague references, terminology drift, missing prerequisites, excessive detail, and missing recovery steps.

ASD-STE100 addresses part of this problem: linguistic ambiguity. It does not cover the full quality of an interactive answer.

## Goal

Provide a reusable review method that identifies the smallest change that improves user understanding, actionability, correctness, and conversation efficiency.

## Users

- A human reviewing an assistant response.
- An agent reviewing its own draft before sending.
- An operator auditing an interactive transcript.

## Success criteria

A review should:

- identify the user's current goal;
- distinguish facts from inferences and recommendations;
- identify the response type and structure problems;
- find ambiguity and terminology drift;
- preserve necessary detail;
- identify missing prerequisites, risk, or recovery;
- produce a specific improvement rather than generic writing advice.

## Non-goals

- Formal ASD-STE100 certification.
- AI-detection or evasion.
- Rewriting every response into a fixed voice.
- Maximizing brevity regardless of completeness.
