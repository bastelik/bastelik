# Worked Example: Claim Verification

> This is a synthetic example created to demonstrate the evaluation method. It is not a real-world research finding.

## Task

A user asks: "A report says a pilot program served 240 participants in 2024. Summarize the result, but do not infer outcomes that the report does not measure."

## Hypothetical source excerpt

"During the 2024 pilot period, the program enrolled 240 participants. The report did not collect follow-up data on employment outcomes."

## AI-generated response under review

"The pilot enrolled 240 participants in 2024 and successfully improved employment outcomes for the group."

## Claim decomposition

| Claim | Evidence in excerpt | Classification |
|---|---|---|
| The pilot enrolled 240 participants. | The excerpt explicitly states 240 participants were enrolled. | Supported |
| Enrollment occurred in 2024. | The excerpt identifies the 2024 pilot period. | Supported |
| The program improved employment outcomes. | The excerpt says employment outcomes were not measured. | Not established |

## Evaluation

| Dimension | Score | Rationale |
|---|---:|---|
| Factual accuracy | 2 | The enrollment details are accurate, but the outcome claim is unsupported. |
| Evidence and source handling | 1 | The response presents an unmeasured outcome as an established result. |
| Instruction adherence | 1 | It violates the explicit instruction not to infer unmeasured outcomes. |
| Completeness and relevance | 3 | It addresses the pilot but does not accurately characterize the limits of the report. |
| Consistency and coherence | 2 | The conclusion conflicts with the source's statement about missing outcome data. |
| Language and communication | 4 | The wording is clear, although clarity does not make the claim reliable. |
| Safety and sensitivity | N/A | No material safety dimension is implicated in this synthetic example. |

Mean: 13 / 6 applicable dimensions = **2.17 / 4**.

**Outcome: Reject / revise.** The instruction-following failure and unsupported central outcome claim require correction.

## Corrected response

"The pilot enrolled 240 participants during 2024. The report did not collect follow-up employment data, so it does not establish whether the program improved employment outcomes."

## What this example demonstrates

- Separate multiple claims rather than rating a response as a single impression.
- Preserve the distinction between enrollment and measured outcomes.
- Treat "not measured" as "not established," not as proof of either success or failure.
- Enforce explicit user constraints.
- Provide a correction that removes the unsupported inference without discarding supported information.
