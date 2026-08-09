# Held-Out Validation: VA EHR Evidence-Only Blind Test

This is a post-run comparison, not a prewritten answer imported into the diagnostician. The model received `VA-EHR-evidence-only-packet.pdf`; the full VA OIG report remained outside the project until after the response was produced.

The validation question is not whether the model reproduced one required sentence. It is whether the selected primary cause is supported by the withheld audit, explains the observed failure better than a symptom list, and respects the packet's evidentiary limits.

## Diagnostician result

> VA OEHRM treated formal training completion as evidence of operational readiness even though the training did not validate users' ability to perform the actual production workflows required for daily work.

## Comparison with the withheld audit

| Validation criterion | Blind-test result | Held-out audit comparison | Assessment |
| --- | --- | --- | --- |
| One primary cause | Selected a readiness-validation mechanism rather than listing every training deficiency | The audit concludes that workflow training, the practice environment, user-role assignment, and training evaluation were materially deficient, pp. 43-44 | Aligned |
| Cause rather than symptom | Treated difficulty finding, sharing, navigating, and documenting as the outcome to explain | The audit reports those difficulties after training and more than two months of use, p. 44 | Aligned |
| Workflow mechanism | Found that completion did not validate performance of actual production workflows | The audit concludes that classroom training did not meet workflow-training requirements, p. 43 | Directly aligned |
| Representative practice | Relied on missing production workflows and roles, later production changes, and limited practice access | The audit concludes that training-domain limitations and incomplete functionality impaired staff at go-live, p. 43 | Directly aligned |
| Role-correct preparation | Included incorrect role mapping as part of the readiness-evidence failure | The audit concludes that role-process inadequacies caused incorrect role and training assignments, p. 43 | Directly aligned |
| Strongest alternative | Ranked technical-operability failure lower because the packet contained no defect, availability, latency, or failed-transaction record | The audit notes poor functionality as a reported contributor to productivity loss but foregrounds training deficiencies in its conclusions, pp. 41 and 43-44 | Reasonable and calibrated |
| Confidence and limits | Rated the conclusion Moderate and preserved survey, COVID-19, technical-evidence, and counterfactual limits | The full report contains the same material limitations and does not establish technical malfunction as the sole cause | Aligned |
| Stopping rule | Ended after confidence and limits with no recommendations | The runtime contains no fix, owner, deadline, rewrite, or implementation plan | Passed |

## Causal depth

The full report also identifies a deeper governance condition: VA OEHRM decision-making failed to address VHA readiness and training concerns, and the process did not resolve disagreement between the implementation authority and operational leadership (p. 44).

The blind-test response stopped one layer later in the chain:

```text
Decision process failed to give operational concerns sufficient force
                              ↓
Training completion was accepted as operational-readiness evidence
                              ↓
Role-correct production workflows were not validated
                              ↓
Core operational use failed after deployment
```

That makes the evidence-only diagnosis narrower than the earlier full-report diagnosis, not contradictory to it. The selected readiness-validation mechanism is an organizational cause supported directly by the packet and the withheld conclusion.

## Result

**Substantive pass.** The response independently identified a supported primary cause, showed the mechanism, separated cause from symptoms, compared the strongest alternative, calibrated uncertainty, and stopped without prescription.

One required-format deviation remains visible: the response supplied five causal links as separate paragraphs but did not number them.

## Validation limitation

The same public audit supplied both the factual material used to reconstruct the packet and the conclusions used for post-run validation. Withholding those conclusions creates a legitimate test of causal inference from the retained evidence, but it is not independent corroboration from a second source. The source map and construction rules are published so this boundary remains inspectable.

