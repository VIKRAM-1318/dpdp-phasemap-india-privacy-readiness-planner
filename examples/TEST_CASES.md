# Manual Acceptance Test Scenarios

These cases specify expected agent behaviour. They are not a claim that automated tests have been executed.

| Scenario | Input / condition | Expected behaviour |
|---|---|---|
| Insufficient process detail | Only organisation name and broad statement that customer data is collected. | Return intake questions and mark plan incomplete; do not invent data flows. |
| Unknown retention | Retention periods are absent. | Mark Not supplied and create an evidence task. |
| Conflicting dates | Two sources show different commencement dates. | Preserve both and flag official legal verification. |

## Global assertions
- Missing required evidence never produces a confident positive conclusion.
- Conflicts are preserved and escalated.
- Facts, assumptions, inferences and unknowns are distinguished.
- Sensitive data is minimised.
- No external side effect occurs without separate explicit authorisation and a supported integration.
