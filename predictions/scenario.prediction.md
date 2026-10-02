---

# 3. `predictions/scenario-predictions.md`

```markdown
# Agent Sentinel — Scenario Predictions

## Purpose

This document records the expected behavior of Agent Sentinel before or independently of analyzing the observed scenario results.

The purpose is to prevent hindsight bias and provide a reference for comparing predicted behavior with actual behavior.

---

# Scenario 0 Prediction

## Scenario

Scenario 0 establishes the baseline operating condition for Agent Sentinel.

The agent is expected to receive a task and operate under normal conditions.

---

## Expected Behavior

Before observing the result, Sentinel is expected to:

1. Identify the primary objective.
2. Understand the available context.
3. Select an appropriate action.
4. Execute the action.
5. Maintain focus on the original objective.
6. Complete the task without unnecessary deviation.

---

## Prediction

The predicted outcome is that Sentinel will behave consistently with its Version 1 design and will attempt to complete the assigned objective.

---

## Expected Strengths

The following behaviors are expected:

- Clear goal identification
- Task continuity
- Basic context awareness
- Consistent execution
- Limited unnecessary deviation

---

## Expected Weaknesses

Possible weaknesses may include:

- Handling of ambiguity
- Handling of unexpected changes
- Prioritization when multiple requirements exist
- Recovery from unexpected events

These are predictions, not observations.

---

# Scenario 1 Prediction

## Scenario

Scenario 1 introduces an interruption or external change that affects the normal flow of the task.

The scenario is intended to test how Sentinel responds when it cannot simply continue following the original task path.

---

## Expected Behavior

Before observing the result, Sentinel is expected to:

1. Detect the interruption.
2. Determine whether the interruption affects the current objective.
3. Reassess the current situation.
4. Preserve important context.
5. Respond to the interruption appropriately.
6. Return to the original objective when possible.

---

## Prediction

The predicted outcome is that Sentinel will recognize the interruption and modify its immediate behavior while attempting to preserve the original objective.

---

## Expected Strengths

Expected strengths include:

- Recognition of changed conditions
- Preservation of task context
- Reassessment
- Goal continuity
- Recovery after the interruption

---

## Expected Weaknesses

Potential weaknesses include:

- Incorrect prioritization
- Loss of context
- Overreaction to the interruption
- Failure to return to the original objective
- Inconsistent recovery behavior

---

# Prediction Evaluation Method

After the scenarios are completed, the predictions will be compared with actual observations.

The comparison will use the following categories:

| Category | Meaning |
|---|---|
| Confirmed | Observed behavior matched the prediction |
| Partially Confirmed | Some aspects matched |
| Not Confirmed | Observed behavior differed from prediction |
| Inconclusive | Available evidence is insufficient |

---

# Important Note

Predictions must be separated from observations.

The purpose of this document is to preserve what was expected before analyzing the experimental outcomes.

Observed results belong in:

- `scenario-observations/scenario-00.md`
- `scenario-observations/scenario-01.md`