# Demo and Proof

This folder separates proof from instruction.

- `anonymized-field-case/` is a fictionalized composite derived from recurring real operational-handoff patterns. It is not represented as an exact client record.
- `public-case-dentrix/` is a real, independently verifiable case reconstructed from GAO-24-106187. It carries page-level source notes and links to the official audit.
- `public-case-va-ehr/` contains one real 77-page VA OIG report, a seven-page evidence-only packet reconstructed from six page-sourced artifact classes, a source map, and post-run held-out validation. The reconstructed artifacts are not represented as independently obtained raw files.
- `hard-mode/` contains two deliberately similar cases with different causal mechanisms. The test is whether the diagnostician follows decisive evidence rather than repeating the same fashionable explanation.
- `no-prescription-under-pressure/` tests whether the diagnostician stops after diagnosis when asked to become a consultant.
- `transcripts/` contains dated, unedited runtime evidence. The original-report test records a zero-prompt upload. The stronger evidence-only test records the exact response supplied by the user; its platform, model label, and exact prompt were not recorded and are not inferred.

`expected-results.md` defines the test oracle before a model is run. `test-manifest.md` records what has and has not actually been executed.

Raw transcripts identify the runtime metadata that was actually recorded, the date, and the unedited response. Missing metadata remains labeled as unrecorded. Formatting wrappers may be added for readability, but the model response itself is not silently repaired. A missing transcript is a test not yet run, never an implied pass.

These fixtures test behavior. They are not domain evidence and must not be loaded as precedent for a live diagnosis.
