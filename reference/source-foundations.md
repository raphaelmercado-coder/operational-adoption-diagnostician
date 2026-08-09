# Source Foundations

This file carries the authoritative source layer behind the diagnostic framework. The sources do not provide a universal formula for adoption. They establish that software transition depends on organizational conditions beyond delivery and that adoption must be evaluated through operating evidence.

Use these sources to constrain reasoning. Do not cite them as evidence that a condition occurred in a specific case. Case conclusions must still come from the supplied evidence packet.

## GAO Agile Assessment Guide

Source: U.S. Government Accountability Office, *Agile Assessment Guide: Best Practices for Agile Adoption and Implementation*, GAO-20-590G, September 2020.  
URL: https://www.gao.gov/assets/gao-20-590g.pdf

Relevant source text:

> "Management should consider the transition to Agile a process improvement or change management effort."

GAO organizes adoption practices across team composition, customer value, repeatable processes, training, technical environment, program controls, organizational activity, and culture. Its reported TSA case is especially important diagnostically: leadership commitment and training were present, yet undefined roles and responsibilities remained material adoption failures.

Diagnostic constraint: training or executive support cannot automatically be named primary merely because adoption failed. Their causal importance must be compared with roles, controls, process, technical environment, and the observed mechanism.

## GAO findings on roles, user involvement, and outcome measures

Source: the supporting case summaries and auditor questions within GAO-20-590G, including GAO-18-46, GAO-19-136, and GAO-20-213.  
URL: https://www.gao.gov/products/gao-20-590g

Relevant source text:

> "The program had not defined key roles and responsibilities."

The guide reports that effective adoption can be undermined when roles are undefined, user involvement lacks required direction, organizational-change actions remain incomplete, or desired outcomes and performance measures are not established.

Diagnostic constraint: distinguish the absence of a role on paper from a demonstrated decision-rights or ownership mechanism. The case packet must connect the governance condition to the failed transition.

## Federal RPA maturity evidence

Source: Federal Robotic Process Automation Community of Practice, *The State of Federal RPA*, Version 2.0, published through Digital.gov.  
URL: https://digital.gov/s3/files/m-files/state-of-federal-rpa-report-12-2021.pdf

Relevant source text:

> "Individual automations may also require various approvals from systems owners, process owners, and other stakeholders."

The report separates production environment, approvals, process improvement, governance, automations in production, program impact, operating metrics, and workload capacity. Its mature-program cases connect deployment at scale with process-owner engagement, defined handoffs, governance, production infrastructure, sustainment, and measured program impact.

Diagnostic constraint: deployment count and technical availability do not independently establish operational adoption. Look for the actor, operating route, sustained production behavior, and impact evidence defined in `adoption-signals.md`.

## How these sources map to this folder

| Source principle | Local diagnostic use |
| --- | --- |
| Adoption is an organizational transition, not only software delivery | The technical-completion and operational-adoption boundary |
| Roles and responsibilities can remain causal despite training and commitment | Decision-rights and ownership-transition hypotheses |
| User involvement and feedback require an explicit operating mechanism | Operating-route and workflow-fit hypotheses |
| Desired outcomes and measures should be established | Outcome-definition and adoption-measurement hypotheses |
| Production, governance, process ownership, sustainment, and impact are distinct | The evidence gate and adoption signals |

## Source discipline

- Preserve the distinction between source-backed general mechanisms and case-specific proof.
- Cite the source URL when invoking a general principle in an explanation.
- Cite case artifacts, not these references, as decisive evidence for the primary cause.
- Do not imply that GAO or the Federal RPA Community of Practice endorses this diagnostician or its taxonomy.
- Do not extend conclusions beyond internal software transitions without additional domain evidence.

