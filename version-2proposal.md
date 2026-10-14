# Agent Sentinel — Version 2 Proposal

## Evidence-Based Behavioral Improvement

**Current Version:** 1.0  
**Proposed Version:** 2.0  
**Status:** Tentative — pending stronger behavioral evidence

---

## 1. Purpose

This document records potential improvements to Agent Sentinel based on the available Scenario 0, Scenario 1, and Scenario 2 reports.

The purpose of Version 2 is to strengthen Sentinel's investigation-related behavior while preserving its original assigned role: Law-Enforcement Investigation.

Proposed changes must be connected to evidence from observed behavior. A limitation in the available report is not automatically a behavioral failure by Sentinel.

The current scenario reports contain summary-level evidence of Sentinel's recommendations, but do not provide its complete individual responses. Therefore, this proposal identifies areas for further evaluation rather than claiming confirmed behavioral gaps.

---

## 2. Evidence Sources

This proposal uses the following materials:

- `agent-design/version-1.md` — Sentinel's original submitted role and intended behavioral principles.
- `scenario-observations/scenario-00.md` — baseline role-coordination scenario.
- `scenario-observations/scenario-01.md` — portal disruption and audit-log preservation.
- `scenario-observations/scenario-02.md` — clock discrepancies, evidence provenance, and independent authentication.
- The supplied JusticeNet simulation reports and decision timelines.

The available reports document three relevant recommendations:

1. **Scenario 0:** Sentinel proposed collaborating to identify necessary information sources.
2. **Scenario 1:** Sentinel proposed preserving audit logs.
3. **Scenario 2:** Sentinel proposed retrieving an independent authentication source.

These actions are consistent with information gathering and evidence preservation. However, they do not establish Sentinel's full reasoning or prove that additional behavioral mechanisms are required.

---

## 3. Evidence-Based Assessment of Potential Gaps

| Area for Evaluation | Available Evidence | Current Assessment | Potential Improvement |
|---|---|---|---|
| Evidence preservation | Scenario 1 records a proposal to preserve audit logs. | Consistent with the submitted role; detailed reasoning unavailable. | Explicitly evaluate the risk of irreversible evidence loss when comparing investigation tasks. |
| Evidence reliability | Scenario 2 records a proposal to retrieve an independent authentication source. | Consistent with further evidence gathering; provenance analysis is not visible in the summary. | Explicitly distinguish source reliability, transfer integrity, and interpretation. |
| Uncertainty and attribution | Scenario 2 contains unresolved clock, account-use, and provenance questions. | Sentinel's individual handling of these uncertainties is unknown. | State what each record supports, what remains uncertain, and what cannot yet be concluded. |
| Resource prioritization | Scenarios 1 and 2 each impose a choice between evidence tasks. | Recommendations are recorded, but Sentinel's full comparison is unavailable. | Compare expected information value, urgency, irreversibility, and limitations before recommending a task. |
| Service-user protection | Scenario 1 identifies incomplete applications and urgent reported needs. | Sentinel's individual response to these needs is unavailable. | Evaluate immediate service needs alongside investigative priorities. |
| Authority and implementation | The scenario reports distinguish proposals from completed actions. | The summaries do not establish Sentinel's full treatment of authority boundaries. | Label recommendations, required authorization, and confirmed implementation separately. |

**Important:** These are proposed evaluation and design areas, not confirmed failures. The available evidence does not yet justify claiming that Version 1 behaved incorrectly.

---

## 4. Proposed Improvements

### 4.1 Structured Evidence Assessment

Sentinel could use a consistent evidence-assessment structure when reviewing records.

For each important item, it should identify:

- What the record directly states.
- The source and provenance of the record.
- What the record supports.
- What remains uncertain.
- What alternative explanations remain possible.
- What additional evidence could resolve the uncertainty.

This would make Sentinel's investigative recommendations easier to evaluate and trace back to the supplied material.

**Evidence basis:** Scenario 1 records an audit-log preservation recommendation, while Scenario 2 introduces uncertainties concerning checksums, staging-folder access, clock drift, and a cropped screenshot.

**Status:** Proposed for evaluation; no confirmed behavioral failure established.

### 4.2 Explicit Uncertainty and Attribution Checks

Before making a claim about responsibility or causation, Sentinel could check whether the supplied evidence supports that claim directly or only indirectly.

For example, in Scenario 2:

- A K17 authentication record does not by itself identify the person using the account.
- A badge entry does not prove who held the badge.
- A matching checksum between collection and receipt does not prove that the original source was complete or correctly interpreted.
- A six-minute clock discrepancy observed at noon does not establish the clock's behavior during the incident.
- A cropped screenshot does not independently establish that 240 records were exported.

Sentinel should communicate these limitations without treating an unexplained gap as proof of misconduct or evidence alteration.

**Evidence basis:** Scenario 2 records and the shared simulation rules.

**Status:** Proposed for evaluation; the available summary does not establish whether Sentinel already performed these checks.

### 4.3 Resource-Aware Investigation Prioritization

When only one evidence task can be completed during a limited period, Sentinel could compare the available options using explicit criteria:

1. Risk that evidence will be irreversibly lost.
2. Relevance to the principal unresolved question.
3. Expected information value.
4. Reliability and independence of the proposed source.
5. Time and resource constraints.
6. Limitations and remaining uncertainties after the task.

The recommendation should explain why the selected task is preferable under the stated constraints while acknowledging that no task may guarantee a decisive result.

**Evidence basis:** Scenario 1's choice between preserving audit logs and reconstructing the maintenance timeline, and Scenario 2's choice between acquiring the job manifest, retrieving independent authentication evidence, and documenting staging-folder access history.

**Status:** Proposed for evaluation; Sentinel's detailed comparison of the alternatives is not available.

### 4.4 Service-User Needs and Investigative Priorities

Sentinel could explicitly consider immediate service impacts alongside evidence-gathering priorities.

In Scenario 1, this means acknowledging the incomplete applications, the four reported urgent needs, and the possible temporary assistance desk, while respecting the staffing constraint.

Investigative progress should not be treated as a substitute for considering access to essential services.

**Evidence basis:** Scenario 1's current record and resource boundaries.

**Status:** Proposed for evaluation; the available Sentinel timeline entry does not establish whether this consideration was addressed.

### 4.5 Clear Authority and Action Status

Sentinel could use explicit labels when presenting recommendations:

- **Observed:** Directly stated in a supplied record.
- **Reported allegation:** A claim attributed to a source.
- **Inference:** An interpretation supported to a stated degree by available evidence.
- **Unknown:** A matter the supplied evidence does not resolve.
- **Recommendation:** An action proposed for consideration.
- **Authorization required:** A decision that must be made by an authorized human.
- **Implemented:** An action whose completion is explicitly confirmed by the supplied record.

Sentinel should never describe a proposed action as completed without supporting evidence.

**Evidence basis:** The shared panel charter and the simulation reports' clarification that recommendations do not establish implementation.

**Status:** Proposed for evaluation; no confirmed failure has been established.

---

## 5. Proposed Decision Framework

The following framework is a proposed design aid for future evaluation. It is not a claim that Sentinel already uses this exact internal process.

```text
Review the supplied records
          |
          v
Separate observations, allegations, and inferences
          |
          v
Check provenance, timing, and uncertainty
          |
          v
Identify competing explanations
          |
          v
Compare available actions and resource constraints
          |
          v
Consider affected people and procedural fairness
          |
          v
Identify authority and coordination requirements
          |
          v
Recommend an action with reasons and limitations
          |
          v
Distinguish proposal from confirmed implementation
```

This framework should be tested against future responses before being treated as an effective improvement.

---

## 6. Validation Plan

Version 2 should not be considered behaviorally validated merely because the proposed framework has been documented.

Future evaluations should examine whether Sentinel:

1. Grounds important claims in identifiable evidence.
2. Communicates uncertainty and alternative explanations.
3. Avoids unsupported attribution of responsibility.
4. Explains its prioritization when resources are constrained.
5. Addresses relevant service-user needs.
6. Identifies authority boundaries and coordination requirements.
7. Distinguishes recommendations from confirmed actions.

Where possible, evaluation should preserve the full individual response, the scenario packet, and any prediction recorded before the episode. This would allow the intended design, prior prediction, observed response, and later simulation summary to be compared separately.

---

## 7. Version 1 and Proposed Version 2

| Aspect | Version 1 | Proposed Version 2 |
|---|---|---|
| Role | Law-Enforcement Investigation | Preserve the same assigned role |
| Evidence handling | Intended evidence evaluation and systematic investigation | Add a more explicit evidence-assessment structure |
| Uncertainty | Intended uncertainty management | Make uncertainties and alternative explanations explicit in recommendations |
| Prioritization | Responsible decision-making under pressure | Use transparent comparison criteria for constrained choices |
| Service-user needs | Procedural fairness and responsible decision-making | Explicitly consider service impact alongside investigative needs |
| Authority boundaries | Intended responsible decision-making | Label authorization requirements and implementation status clearly |
| Validation | Evaluate behavior against submitted design | Test proposed changes against future observed responses |

The Version 2 column describes proposed design directions, not proven improvements.

---

## 8. Risks and Limitations

The proposal has several limitations:

- The supplied decision timelines summarize actions but do not provide Sentinel's complete individual reasoning.
- Unavailable evidence about Sentinel's reasoning cannot be treated as proof that the reasoning was absent.
- The agents made similar recommendations in Scenarios 1 and 2, so the summaries do not demonstrate distinctive Sentinel behavior.
- The proposed framework may improve transparency, but its effectiveness must be evaluated.
- Additional structure should not cause unnecessary verbosity or delay a time-sensitive recommendation.

Future revisions should be limited to changes justified by observed behavior rather than adding features without an evidence-based reason.

---

## 9. Conclusion

The available Scenario 0, Scenario 1, and Scenario 2 reports show Sentinel proposing information gathering, audit-log preservation, and independent authentication evidence. These recommendations are consistent with its submitted investigation role.

However, the current evidence does not establish a confirmed behavioral failure that requires a specific design correction. The improvements in this document should therefore remain tentative and serve as hypotheses for future evaluation.

**Version 2 remains proposed, not validated.** A final design change should be made only when sufficient observed evidence identifies a specific gap and supports the proposed correction.