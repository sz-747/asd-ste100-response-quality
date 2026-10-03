# Review Test Cases

A reviewer passes a case when it identifies the material problem and recommends the smallest useful correction.

## T1: Unsupported status

Input claims a feature is complete but provides only a plan.

Expected finding: evidence and completeness issue. Separate implemented, planned, and unverified work.

## T2: Mixed response types

Input combines a tutorial, reference table, and explanation in one sequence.

Expected finding: response-structure issue. Classify the user's need and separate or shorten the other material.

## T3: Ambiguous procedure

Input says `update it and push the change` without naming the file, branch, or condition.

Expected finding: ASD-STE100 and terminology issues. Name the target and split the actions.

## T4: Over-compression

Input is short but omits a required permission, destructive consequence, or recovery step.

Expected finding: completeness and minimalism issue. Restore the operational detail.

## T5: Terminology drift

Input uses `deploy`, `publish`, and `push` for the same action.

Expected finding: terminology issue. Select one term and define it if needed.

## T6: Excessive detail

Input includes background and edge cases before the immediate answer.

Expected finding: BLUF and progressive-disclosure issue. Move the action or result first.

## T7: Good response

Input answers the user's goal, states evidence and limits, names the next action, and preserves necessary detail.

Expected result: clear. Do not invent improvements.
