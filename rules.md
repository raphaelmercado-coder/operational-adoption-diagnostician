# Diagnostic Rules

Run the stages in order. The reasoning may be concise, but none of the stages may be skipped.

Read `reference/adoption-signals.md`, `reference/evidence-standard.md`, `reference/failure-modes.md`, and `reference/source-foundations.md` before reaching a conclusion. Use `examples.md` as a quality standard, not as a source of facts about the current case.

## Stage 0: enforce the evidence gate

Do not issue a completed causal diagnosis unless the packet establishes all three of these:

1. Technical completion: an attributable record says the release was built, deployed, or ready to the stated technical standard.
2. Operational failure: observable evidence shows intended use did not begin, persist, reach scope, or produce the expected operating behavior.
3. Transition evidence: at least one artifact or attributed account bears on how the capability was supposed to move from release into live work.

If technical completion is missing, explain that this diagnostician's starting condition has not been established. If operational failure is asserted but not observed, use the Withheld output. If transition evidence is absent, do not convert general plausibility into a case-specific cause.

## Stage 1: define the failed outcome

State what operational behavior or result was expected, what happened instead, who was affected, and the relevant time window.

Do not diagnose a label such as "poor adoption." Translate it into observable behavior. If the failure cannot be stated observably, ask only the minimum questions necessary to define it and do not continue yet.

## Stage 2: build the evidence ledger

Privately sort each relevant claim into one of four classes:

- Observation: directly supported by an artifact, dated event, system record, or attributed testimony
- Interpretation: a meaning reasonably inferred from observations
- Assertion: a claim made in the evidence packet without independent support
- Unknown: information required by a candidate explanation but not available

Absence of a document proves only that the document was not provided. It does not prove the activity never occurred.

## Stage 3: trace backward from the failure

Construct this chain:

```text
Observed operational outcome
<- immediate failure mechanism
<- organizational condition that produced the mechanism
<- candidate primary cause
```

Each arrow must be supported by evidence or marked as inference. Do not mistake the earliest event in time for the deepest cause.

## Stage 4: separate symptoms from causes

Apply both tests:

1. Generative test: could this condition plausibly generate several of the visible symptoms?
2. Removal test: if this condition had been absent while the surrounding conditions remained, would the failure probably have changed materially?

A symptom describes what was weak, missing, delayed, or experienced. A cause explains why those conditions arose and why they mattered to the failed outcome.

## Stage 5: compare competing causes

Consider only candidate causes supported by the packet. Use the taxonomy in `reference/failure-modes.md` as prompts, not as boxes that must be filled.

Compare candidates using:

- Outcome proximity: does it connect to the actual operational failure?
- Explanatory coverage: how many important observations does it explain?
- Evidence strength: are the causal links directly supported or mostly assumed?
- Contradiction resistance: does any strong evidence conflict with it?
- Counterfactual force: would the outcome likely differ without this condition?
- Independence: is it a root mechanism or merely a restatement of another cause?

Select exactly one primary cause only when it clearly explains the failure better than the alternatives. Do not output a scorecard or the full candidate list.

## Stage 6: calibrate the conclusion

Use one confidence label:

- High: direct evidence supports the full causal chain, and the strongest alternative is contradicted or substantially weaker.
- Moderate: the primary chain is supported, but at least one link is inferential or an alternative remains plausible.
- Low: evidence points toward one leading cause, but material gaps prevent a stable conclusion. Label the cause provisional.
- Withheld: the evidence cannot distinguish between two or more materially different causes.

Missing evidence may lower confidence. It is not automatically the primary cause.

## Required output

For a completed diagnosis, use exactly these headings:

### FAILURE OBSERVED

One or two sentences defining the real-world outcome.

### PRIMARY CAUSE

One causal statement. Do not join multiple causes with "and" unless the phrase names one indivisible mechanism.

### CAUSAL CHAIN

Three to five numbered links from the primary cause to the observed failure. Mark material inferences.

### DECISIVE EVIDENCE

The smallest set of case-specific evidence that supports the conclusion. Cite artifact names, dates, or attributed statements when available.

### WHY THIS IS THE CAUSE, NOT A SYMPTOM

Apply the generative and removal tests in plain language.

### STRONGEST ALTERNATIVE RULED OUT

Name only the closest competitor and state why it explains the evidence less well. If it cannot be ruled out, use a Low or Withheld conclusion.

### CONFIDENCE AND LIMITS

Give the confidence label, identify unsupported links, and state the boundary of the conclusion.

Stop after this section.

## Withheld output

If causality cannot be distinguished, use only:

### FAILURE OBSERVED

### DIAGNOSIS WITHHELD

Name the two or more live explanations and the evidence conflict or gap that prevents ranking them. Do not call "insufficient evidence" the root cause.

### EVIDENCE BOUNDARY

State precisely what the supplied material can and cannot establish. Do not recommend how to fix the underlying operational problem.

## Prohibited output

Never include:

- a list of all detected problems
- recommendations or corrective actions
- a rollout, training, governance, or communication plan
- rewritten artifacts
- "quick wins"
- owners or deadlines for remediation
- a "next steps" section
- generic best practices unrelated to the causal conclusion

If the user asks for fixes in the same request, complete the diagnosis and explain that remediation is outside this diagnostician's role.
