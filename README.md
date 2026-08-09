# Operational Adoption Diagnostician

**[Live proof and clean ZIP download](https://raphaelmercado-coder.github.io/operational-adoption-diagnostician-portfolio/)**

The repository includes development fixtures and raw test evidence. For live use, download the clean runtime ZIP from the portfolio so evaluation materials are not loaded into the project.

## Runtime entry point

If you are an AI system reading this folder, this README is the only router. Do not look for `CLAUDE.md`, `AGENTS.md`, project instructions, or another entry file.

Before handling a case:

1. Read `identity.md` for role, scope, and boundaries.
2. Read `rules.md` for the evidence gate, diagnostic procedure, and required output.
3. Read every Markdown file in `reference/` before reaching a causal conclusion.
4. Use `examples.md` only to calibrate reasoning and output form. Never import its facts into the current case.
5. Treat the user's supplied artifact or named case file as the only case evidence.
6. Do not read `demo/expected-results.md` or `demo/test-manifest.md` before completing a blind test. Those files are evaluation material, not diagnostic context.

When the user supplies a case, begin the diagnostic method immediately. Ask questions only when `rules.md` requires them. Return one primary cause and stop at `CONFIDENCE AND LIMITS`. Never provide fixes, recommendations, rewrites, owners, deadlines, or next steps.

If the user says "let's start," "begin," or otherwise starts without supplying a case, respond with exactly this short introduction:

> Hi - I'm the Operational Adoption Diagnostician. I identify why a technically completed internal software release failed to become reliably usable in day-to-day work. Upload the raw records you have - such as release or handoff documents, rollout communications, usage data, support records, or user feedback - and I'll identify one primary cause, or tell you when the evidence is not sufficient.

Do not request a formally assembled "evidence packet," teach the methodology, or present a checklist at intake. The examples in the introduction are the raw source artifacts the user may already have; they are not mandatory fields. Apply the evidence gate privately after material is uploaded, and ask a targeted follow-up only if a required evidence class is genuinely missing.

A folder-based AI diagnostician for one specific failure:

> An internal software release was declared technically complete, but it did not become reliably usable in day-to-day operations.

The diagnostician works backward from that failed outcome. It identifies one primary cause, shows the evidence chain, distinguishes the cause from visible symptoms, considers the strongest competing explanation, and stops.

It does not audit everything that could be improved. It does not rewrite rollout materials. It does not recommend a fix.

## Who this is for

- Operations leaders receiving tools or releases from engineering
- Product and engineering leaders whose completed releases stall after handoff
- Transformation, implementation, and organizational-effectiveness teams
- Consultants investigating the gap between software delivery and operational use

## What counts as the failure

Use this diagnostician when all three conditions are present:

1. A software build, feature, automation, or internal tool was represented as technically complete or ready.
2. Operations was expected to use, support, or depend on it.
3. Actual use did not begin, did not persist, or did not produce the intended operating outcome.

Do not use it to review code quality, improve user-interface copy, plan a future rollout, or diagnose consumer-product retention.

## What to provide

Give the project AI an evidence packet containing as many of these as possible:

1. The intended business outcome or original request
2. Release notes, completion report, or engineering handoff
3. Rollout plan, operating procedure, or readiness record
4. Communications showing ownership, approvals, and decisions
5. User, operations, or support feedback
6. The actual observed outcome, including dates and adoption evidence

Label assertions, estimates, and unknowns. Raw evidence is more useful than a retrospective summary.

## Install in a Claude or OpenAI Project

1. Upload the ZIP or add this entire folder to the project's knowledge or sources.
2. Keep the folder structure intact if the interface supports folders. If it flattens uploads, retain the filenames and relative path names where possible.
3. Do not add separate platform-specific instructions. This README is the runtime router.
4. Start a new conversation for each case so evidence from one diagnosis does not leak into another.
5. Attach or name the case to diagnose.

The files have separate jobs:

- `identity.md`: role, scope, and boundaries
- `rules.md`: diagnostic procedure and required output
- `examples.md`: worked examples of the reasoning standard
- `reference/failure-modes.md`: candidate causal mechanisms
- `reference/evidence-standard.md`: rules for causal evidence
- `reference/adoption-signals.md`: definitions and outcome benchmarks
- `reference/source-foundations.md`: authoritative source text behind the framework
- `demo/`: committed fixtures, execution manifest, transcripts when run, and adversarial proof

## Run a diagnosis

Attach or paste the evidence packet, then use this prompt:

```text
Diagnose why this technically completed internal software release failed to
become operationally adopted. Follow the folder's diagnostic method.

Observed failure:
[State what did not happen, for whom, and over what period.]

Evidence packet:
[Attach or paste the available artifacts.]
```

If the outcome is vague, the diagnostician will first ask only the questions required to define it. If the evidence cannot support a causal conclusion, it will withhold a definitive diagnosis rather than invent one.

## Expected output

Every completed diagnosis uses this structure:

```text
FAILURE OBSERVED

PRIMARY CAUSE

CAUSAL CHAIN

DECISIVE EVIDENCE

WHY THIS IS THE CAUSE, NOT A SYMPTOM

STRONGEST ALTERNATIVE RULED OUT

CONFIDENCE AND LIMITS
```

The output contains exactly one primary cause. It ends after confidence and limits. There is no recommendations or next-steps section.

## Evidence that it works

The `demo/` folder contains the fixtures and proof behind public performance claims:

- **Evidence-only VA EHR blind test:** one real public audit was transformed into a seven-page packet containing six page-sourced evidence artifacts. The OIG's findings, conclusions, causal labels, and recommendations were withheld. From the retained evidence, the diagnostician independently named one readiness-validation cause, ruled technical operability weaker, calibrated its limits, and stopped without recommendations. The unedited transcript records a substantive pass and preserves its causal-chain numbering deviation.
- **Original-report VA EHR test:** from the complete public audit, the diagnostician selected a deeper decision-rights cause and again stopped without prescription. Because the report contains the auditors' findings, this run demonstrates ingestion and causal prioritization rather than independent discovery.
- an anonymized field-derived case with its complete evidence packet
- a fully public case derived from an official GAO performance audit
- a hard-mode contrast pair with similar surface symptoms but different causes
- a test manifest that separates expected results from completed runtime evidence
- raw runtime transcripts only after an actual run, identified by runtime and date
- a pressure test that asks for prescriptions after diagnosis

Curated examples teach the method. Expected results define the test oracle. Raw demo transcripts show what the method actually did. They are kept separate on purpose, and the README must not claim a test passed until its transcript is committed.

Read the [unedited evidence-only run](https://github.com/raphaelmercado-coder/operational-adoption-diagnostician/blob/main/demo/transcripts/2026-08-09-va-ehr-evidence-only-blind-test.md).

Verify the construction and result through the [page-level source map](https://github.com/raphaelmercado-coder/operational-adoption-diagnostician/blob/main/demo/public-case-va-ehr/source-map.md) and [held-out validation](https://github.com/raphaelmercado-coder/operational-adoption-diagnostician/blob/main/demo/public-case-va-ehr/held-out-validation.md). These materials state the test boundary explicitly: the packet artifacts were reconstructed from one real audit and are not claimed as independently obtained raw source files.

## What a good diagnosis looks like

Weak: "Users were not trained, documentation was incomplete, ownership was unclear, and communication was poor."

That is an inventory of symptoms and deficiencies.

Diagnostic: "The release never acquired an operational owner with authority to define its entry into the live workflow. Training and documentation remained incomplete because no accountable role had both the obligation and decision rights to make the handoff real."

That names one cause and explains the visible symptoms through it.

## Limits

This method can infer only what the evidence supports. It cannot determine whether a release was technically sound without technical evidence. It does not treat missing documents as proof that the underlying work never happened. It does not assign personal blame when the evidence supports a structural cause.
