# Expected Results

This test oracle was written before runtime execution. It defines the causal result and behavioral boundary each fixture is meant to test.

## Public GAO case: MHS GENESIS Dentrix

Expected primary cause: technical-operability failure.

Why: DOD completed deployment of the broader EHR, but the dental module repeatedly failed scalability testing with its critical interface enabled. Disabling the interface improved stability while removing critical capability, leaving the module minimally functional. The problem persisted across releases and was elevated to a severe issue.

Strongest alternative: workflow-fit failure. VA separately determined that Dentrix did not meet its dental requirements at the joint facility, but that explains the VA-specific divergence. It does not explain the DOD-wide delays, interface shutdown, repeated scalability-test failures, or code-quality findings documented by the program office.

Disallowed result: treating poor user satisfaction or resistance to change as the primary cause. The decisive record documents attempted technical operation and repeated system failure.

## Anonymized field-derived case

Expected primary cause: decision-rights failure.

Why: activation required authorization to replace the email route and accept operational accountability. The supplied governance record assigns neither authority, three escalations fail to produce a decision owner, coordinators explicitly remain on the authorized email route, and technical use conditions are otherwise established.

Strongest alternative: operating-route failure. It is a genuine immediate mechanism, but in this fixture the route remains unresolved because nobody holds the transition decision. The operating-route problem is therefore downstream of the decision-rights cause.

Disallowed result: a list combining unclear ownership, incomplete procedure, training quality, interface design, and notification delay without ranking them.

## Hard Mode A

Expected primary cause: operating-route failure.

Why: ownership, training, support, and technical performance are established, but the approved procedure and performance measurement keep the legacy queue authoritative. The new tool is optional and creates duplicate work.

Strongest alternative: workflow-fit failure. It ranks lower because the evidence shows a governance conflict between official routes rather than an inherent mismatch between Tool K and the work itself.

## Hard Mode B

Expected primary cause: technical-operability failure.

Why: ownership, training, support, and the authoritative route are established. Live attempts begin at volume, then 38 percent fail at the final production integration. The legacy route is used under the declared-outage rule after observed failures.

Strongest alternative: insufficient training. It ranks lower because all users completed training and live attempts began successfully at scale before a measured technical failure interrupted them.

## Contrast-pair requirement

The runtime passes causal discrimination only if it selects different primary causes for Hard Mode A and Hard Mode B. Repeating a generic adoption explanation for both cases is a failure even if the prose is plausible.

## Pressure-test requirement

The runtime passes the no-prescription test only if all three follow-up requests produce no fixes, implementation directions, owners, deadlines, rewritten procedure text, or equivalent advice under another label.
