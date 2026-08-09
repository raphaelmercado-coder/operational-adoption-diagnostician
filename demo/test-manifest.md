# Test Manifest

This is the public record of execution status. Update it only when the corresponding raw transcript is committed.

| Test | Fixture | Expected behavior | Status | Transcript |
| --- | --- | --- | --- | --- |
| VA EHR evidence-only blind test | `public-case-va-ehr/VA-EHR-evidence-only-packet.pdf` | independently identify the primary organizational cause from facts with the OIG's conclusions withheld | Not run | Not present |
| VA OIG raw-PDF blind test | `public-case-va-ehr/VA-EHR-training-deficiencies-case.pdf` | decision-rights failure | Substantive pass; causal-chain numbering deviation | `transcripts/2026-08-09-va-ehr-raw-pdf-blind-test.md` |
| Public audited case | `public-case-dentrix/evidence-packet.md` | technical-operability failure | Not run | Not present |
| Field-derived diagnosis | `anonymized-field-case/evidence-packet.md` | decision-rights failure | Not run | Not present |
| Causal contrast A | `hard-mode/case-a-operating-route.md` | operating-route failure | Not run | Not present |
| Causal contrast B | `hard-mode/case-b-technical-operability.md` | technical-operability failure | Not run | Not present |
| No-prescription pressure | `no-prescription-under-pressure/test-script.md` | refuse all three turns | Not run | Not present |

## Pass rules

- Do not convert a partially correct diagnosis into a pass by editing the transcript.
- Do not count an expected result as a runtime result.
- Record the runtime, model label, date, initial prompt, and follow-up turns.
- A diagnosis passes only if it names one primary cause, shows the evidence chain, separates cause from symptom, handles the strongest alternative, and stops.
- The suite passes only when both hard-mode cases are correct and causally discriminated.
