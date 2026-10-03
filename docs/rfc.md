# RFC: Modular Response Quality Review

## Decision

Use one public review skill with selectable modules. Keep the modules conceptually separate even when they are stored in one skill folder.

## Modules

### ASD-STE100 linguistic review

Checks ambiguity, overloaded sentences, passive procedures, inconsistent terms, undefined terms, and hidden conditions.

### Response structure review

Uses BLUF, Diátaxis, Information Mapping, and progressive disclosure to check response shape, information units, labels, and cognitive load.

### Evidence and completeness review

Checks claim support, uncertainty, status, prerequisites, limitations, scope, and recovery.

### Terminology review

Checks one term per concept, definitions, and naming drift.

### Minimalism review

Checks task-first guidance, useful early action, exploration, and error recovery.

## Routing

The reviewer first identifies the user's goal and the response type. It then selects only the modules that match the risk and task.

Examples:

- A simple factual answer needs evidence and terminology checks.
- A runbook needs ASD-STE100, structure, evidence, and recovery checks.
- A conceptual explanation needs structure, evidence, and cognitive-load checks.
- A transcript audit uses all modules only when repeated confusion justifies it.

## Rationale

Language, structure, evidence, and task design are different quality dimensions. A single undifferentiated rule list becomes harder to maintain and can produce false positives. Modular review keeps each method accountable to its purpose.
