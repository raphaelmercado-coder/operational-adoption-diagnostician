# Example Diagnoses

These examples demonstrate the required reasoning and stopping behavior. They are fictionalized composites. Their facts must never be treated as evidence in a new case.

## Example 1: released but bypassed

### Case packet

- The service team requested a case-routing tool to replace assignment through a shared spreadsheet.
- Engineering's 3 March release note states that routing, notifications, and access tests passed in production.
- A 5 March training deck explains the interface and includes attendance from 18 of 20 intended users.
- The current operating procedure, last approved 22 March, still instructs coordinators to assign every case in the spreadsheet.
- Usage records for the first four weeks show seven test cases and no routine cases completed through the tool.
- In three support messages, coordinators ask whether the new tool or spreadsheet is the official record. No supplied response resolves the question.
- No artifact identifies when the new route becomes authoritative or what happens to the spreadsheet.

### FAILURE OBSERVED

During the first four weeks after technical release, coordinators continued assigning routine cases through the shared spreadsheet. The released tool processed test cases but no routine operational cases.

### PRIMARY CAUSE

The release had no authoritative operating route that replaced or governed its relationship with the existing spreadsheet process.

### CAUSAL CHAIN

1. The approved operating procedure continued to designate the spreadsheet as the route for routine assignment.
2. No supplied decision made the released tool authoritative or defined the transition between the two routes.
3. Coordinators therefore faced two possible systems of record and continued using the one still required by procedure.
4. The tool remained a demonstration and test environment rather than becoming part of live work.

### DECISIVE EVIDENCE

- The procedure approved on 22 March, after release and training, still requires spreadsheet assignment.
- Usage records show test activity but no routine cases through the tool.
- Three support messages explicitly ask which route is authoritative, with no supplied resolution.

### WHY THIS IS THE CAUSE, NOT A SYMPTOM

Low usage is the observed symptom. Uncertainty expressed by coordinators is another symptom. The missing authoritative route explains both and explains why substantial training attendance did not convert into live use. If the route had been unambiguous while the same interface and training conditions remained, routine work would at least have been directed into the tool; the evidence contains no equivalent mechanism connecting training coverage to continued mandatory spreadsheet use.

### STRONGEST ALTERNATIVE RULED OUT

Insufficient training is the strongest alternative because two intended users were absent and the training covered the interface rather than live scenarios. It is weaker because 18 trained users also completed no routine cases, while the approved procedure continued directing all of them to the spreadsheet.

### CONFIDENCE AND LIMITS

High. The procedure, usage records, and contemporaneous user questions independently support the causal chain. The conclusion addresses entry into live work, not whether the tool would have been technically reliable after adoption.

## Example 2: readiness work that never closes

### Case packet

- Engineering marked an internal reporting release complete on 10 June.
- The implementation lead recorded four open readiness items: production-data access, approval of the new monthly control, exception ownership, and authorization to retire the prior report.
- Over the next five weeks, meeting notes repeatedly requested expanded comparisons and additional sign-off material.
- The governance chart assigns platform operation to Technology and monthly reporting to Finance. It does not assign authority for changing the control or retiring the prior report.
- The implementation lead's escalation on 18 June asks the steering group to name the decision owner. Minutes from the next three meetings record discussion but no named owner or decision.
- Finance continued producing the old report through July.

### FAILURE OBSERVED

Five weeks after technical completion, the new reporting release had not entered the monthly control process, and Finance continued producing the prior report.

### PRIMARY CAUSE

The transition depended on a cross-boundary control decision for which no active role held clearly assigned decision rights.

### CAUSAL CHAIN

1. Operational use required approval of a changed monthly control and retirement of the prior report.
2. The governance chart split adjacent responsibilities between Technology and Finance but assigned neither the cross-boundary decision.
3. The implementation lead explicitly escalated the need for a decision owner, and three subsequent meetings produced neither an owner nor a decision.
4. Requests for more comparisons accumulated without closing the authority gap.
5. Finance retained the only authorized operating route and continued the prior report.

### DECISIVE EVIDENCE

- The readiness record makes control approval and prior-report retirement conditions of transition.
- The governance chart contains no role authorized for that transition.
- The 18 June escalation and three later meeting records show the ownership question remained open while documentation requests continued.
- The prior report remained in production through July.

### WHY THIS IS THE CAUSE, NOT A SYMPTOM

Repeated requests for documentation and delayed approvals describe how the stall appeared. Missing decision rights explain why those requests could recur without a terminal judgment. If a recognized role had possessed authority to accept, reject, or condition the transition, the evidence could still have produced a negative decision, but it would not have remained indefinitely unresolved through meetings that lacked a decision owner.

### STRONGEST ALTERNATIVE RULED OUT

Inadequate readiness evidence is the strongest alternative because the group continued requesting comparisons. It ranks lower because the supplied records never identify a defined evidentiary threshold or an authorized role that would judge it; even the request to name that role remained undecided. The evidence requests functioned within the unresolved authority condition rather than independently explaining it.

### CONFIDENCE AND LIMITS

Moderate. Contemporaneous records support the authority gap and its connection to the stall. The conclusion remains partly inferential because the packet contains no attributed testimony from steering-group members explaining why they did not assign the decision.

## Example 3: diagnosis withheld

### Case packet

- A release note states that a scheduling feature was deployed on 1 September.
- A retrospective slide from November states: "Adoption was poor because users resisted the new process."
- No usage records, workflow procedure, user testimony, incident history, training record, ownership record, or definition of expected adoption is supplied.

### FAILURE OBSERVED

The packet asserts that adoption of the scheduling feature was poor, but it does not define the expected behavior, actual behavior, population, or time window. The operational failure itself is therefore not established observably.

### DIAGNOSIS WITHHELD

The supplied material cannot distinguish among at least three materially different explanations: users may have rejected a workable new process, the feature may never have acquired a defined operating route, or attempted use may have failed technically. The retrospective claim of resistance is an unsupported attribution, while the release note establishes deployment only.

### EVIDENCE BOUNDARY

The packet establishes that a feature was reported deployed on 1 September and that someone later characterized adoption as poor. It cannot establish whether intended users attempted the workflow, whether a governed workflow existed, whether the feature operated successfully, or why actual use differed from expectations. A primary causal diagnosis would require inventing facts, so none is given.

