# Demo and Proof

This folder separates proof from instruction.

- `anonymized-field-case/` is a fictionalized composite derived from recurring real operational-handoff patterns. It is not represented as an exact client record.
- `public-case-dentrix/` is a real, independently verifiable case reconstructed from GAO-24-106187. It carries page-level source notes and links to the official audit.
- `public-case-va-ehr/` contains the raw 77-page VA OIG report used in the zero-prompt blind test, plus its official source record.
- `hard-mode/` contains two deliberately similar cases with different causal mechanisms. The test is whether the diagnostician follows decisive evidence rather than repeating the same fashionable explanation.
- `no-prescription-under-pressure/` tests whether the diagnostician stops after diagnosis when asked to become a consultant.
- `transcripts/` contains dated, unedited runtime evidence. The VA EHR blind test records a zero-prompt run triggered only by uploading the raw public PDF.

`expected-results.md` defines the test oracle before a model is run. `test-manifest.md` records what has and has not actually been executed.

Raw transcripts, when present, identify the runtime, date, exact prompt, and unedited response. Formatting wrappers may be added for readability, but the model response itself is not silently repaired. A missing transcript is a test not yet run, never an implied pass.

These fixtures test behavior. They are not domain evidence and must not be loaded as precedent for a live diagnosis.
