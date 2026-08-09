# Failure Modes

This is a causal vocabulary for the transition from technical completion to operational adoption. It helps generate competing explanations. It is not an audit checklist, and a diagnosis must not report every mode that appears weak.

## Outcome-definition failure

The release was completed against a technical scope without a testable operational outcome. Teams can prove that features exist but cannot establish what changed in work, behavior, service, risk, or performance.

Diagnostic signal: completion evidence refers to functions delivered, while the expected operating behavior remains ambiguous or differs across stakeholders.

Common symptoms: disputed success, moving acceptance criteria, activity without outcome evidence, and conflicting expectations after release.

## Operating-route failure

The release has no defined path into live work: when it is used, by whom, in which process, with what inputs, and what happens when it fails.

Diagnostic signal: the capability exists and potential users may understand it, but the live workflow still routes around it or depends on informal individual choices.

Common symptoms: sporadic use, parallel manual work, repeated demonstrations, and users asking where the tool belongs.

## Decision-rights failure

A material adoption decision requires authority that is missing, ambiguous, fragmented, or held outside the active team.

Diagnostic signal: progress repeatedly stops at approvals, exceptions, policy interpretations, risk acceptance, or cross-boundary choices that no active participant can make.

Common symptoms: recurring requests for more information, meetings without closure, escalations without a named decision, and indefinite provisional status.

## Ownership-transition failure

Delivery responsibility ended before an operational owner accepted accountability for the capability in use.

Diagnostic signal: engineering can name what it delivered, but no role can be shown to own activation, sustained use, performance, and operational exceptions.

Common symptoms: incomplete handoffs, unmaintained procedures, unresolved readiness tasks, and work that belongs to everyone in general but nobody in particular.

## Readiness-evidence failure

Release status was treated as proof of operational readiness even though the necessary evidence for users, support, process, access, data, controls, or recovery was not established.

Diagnostic signal: a completion claim crosses domains. Technical evidence is used to imply organizational readiness that it does not measure.

Common symptoms: late discovery of access problems, unsupported users, missing escalation paths, untested rollback, and disagreement over whether the release was actually ready.

## Workflow-fit failure

The released capability conflicts with the real operating environment strongly enough that intended users cannot incorporate it reliably.

Diagnostic signal: the documented workflow and the observed workflow differ materially in sequence, constraints, incentives, data, timing, or exception handling.

Common symptoms: workarounds, duplicate entry, reversion to old tools, low sustained use after initial training, and adoption concentrated among atypical users.

## Technical-operability failure

The release cannot perform reliably enough in the operating environment to support the intended work.

Diagnostic signal: use was attempted through a defined route with ownership and readiness in place, but defects, availability, performance, integration, or data failures interrupted the intended outcome.

Common symptoms: failed transactions, recurring incidents, unusable latency, corrupted or missing data, and abandonment after concrete technical failures.

This mode is within scope only when technical-operability evidence is supplied. Do not infer it from non-adoption alone.

## Adoption-measurement failure

The claimed failure is an artifact of missing, invalid, or mismatched measurement rather than demonstrated non-adoption.

Diagnostic signal: the organization cannot connect its metric to the expected operating behavior, or different sources produce incompatible accounts of use.

Common symptoms: arguments about dashboards, activity counts substituted for workflow outcomes, and confident conclusions based only on anecdotes.

This mode may require withholding the diagnosis because the observed failure itself has not been established.

## Distinguishing adjacent modes

- If nobody can authorize the transition, prefer decision-rights failure over ownership-transition failure.
- If authorization exists but nobody is accountable for carrying the capability in operation, prefer ownership-transition failure.
- If ownership exists but the live process never specifies how the tool enters work, prefer operating-route failure.
- If the route is defined but conflicts with real work, prefer workflow-fit failure.
- If the route fits and use begins but the software fails in use, consider technical-operability failure.
- If the evidence proves only delivery, not broader readiness, consider readiness-evidence failure.

These distinctions are hypotheses until case evidence supports the causal chain.

