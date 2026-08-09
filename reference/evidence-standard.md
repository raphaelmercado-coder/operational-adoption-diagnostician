# Evidence and Causality Standard

The diagnostician explains an observed outcome. It does not reward the most plausible story; it selects the causal explanation best supported by the supplied record.

## Evidence hierarchy

Use this hierarchy as a guide, not an automatic scoring formula:

1. Direct behavioral or system evidence: usage events, workflow records, incidents, timestamps, transaction outcomes
2. Contemporaneous artifacts: approved requirements, release records, decision logs, handoffs, procedures, support records
3. Attributed testimony: dated statements from people who performed, supported, or governed the work
4. Retrospective summaries: later accounts of what happened
5. Unattributed interpretation: claims without a named source or observable basis

Corroboration across independent sources is stronger than repetition of the same original claim.

## Four claim classes

### Observation

A case-specific fact directly supported by the supplied material.

Example: "The release record marked Build A complete on 4 May. The operating procedure dated 9 May still directs staff to the prior manual process."

### Interpretation

A meaning inferred from one or more observations.

Example: "The released capability had not been incorporated into the governed workflow."

### Assertion

A claim contained in the packet whose supporting basis is not supplied.

Example: "Everyone was trained," stated in a retrospective email without attendance, assessment, or observed-use evidence.

### Unknown

A fact needed to evaluate a live causal explanation but not established by the packet.

Example: whether users attempted the defined process and encountered technical errors.

Do not silently promote assertions or unknowns into observations.

## Causal sufficiency

A primary cause should satisfy four conditions:

1. Precedence: the condition existed before or during the failed transition.
2. Mechanism: there is a credible path from the condition to the observed outcome.
3. Coverage: the condition explains the central evidence, not merely one detail.
4. Discrimination: it explains the case better than the strongest materially different alternative.

Temporal precedence alone is not causality. A missing artifact alone is not causality. A recurring correlation alone is not causality.

## The generative test

A cause should generate downstream observations. For example, absent decision rights can generate delayed approvals, repeated document requests, provisional work, and meetings without closure. Those observations may therefore be symptoms of the same mechanism.

If a proposed cause merely renames one symptom, it fails this test.

## The removal test

Ask whether the failure probably changes if the proposed condition is removed while other major conditions remain.

If training materials were complete but nobody could authorize live use, the release would likely remain stalled. Missing training is therefore unlikely to be primary in that case.

This is a disciplined counterfactual, not proof. State when it relies on inference.

## Negative evidence

Treat absence carefully:

- "No owner is named in any supplied artifact" is an observation about the packet.
- "There was no owner" is a conclusion requiring corroboration.
- "The missing owner caused non-adoption" requires a mechanism connecting ownership to the outcome.

Ask whether the artifact would normally record the fact. Missing approval in an approval log is more probative than missing approval in release notes.

## Conflicting evidence

When sources conflict:

1. Preserve both claims.
2. Compare proximity to the event, source competence, contemporaneity, and independent corroboration.
3. Do not resolve the conflict by choosing the more detailed narrative.
4. Lower confidence or withhold the diagnosis if the conflict determines which cause is primary.

## Personal blame

Do not infer unwillingness, incompetence, resistance, or bad intent from structural evidence. "The operations lead resisted change" requires evidence of behavior and still may describe a response rather than the condition that generated it.

## Citation discipline

In the decisive-evidence section, cite the smallest case-specific set needed to support the chain. Name the artifact, date, record, or attributed source. Do not bury the diagnosis under an evidence inventory.

