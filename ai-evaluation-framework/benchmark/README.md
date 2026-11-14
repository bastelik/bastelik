# LLM Evaluation Benchmark

This benchmark is a small, reproducible demonstration set for evaluating response quality against explicit task requirements and reference evidence.

**Dataset type:** synthetic demonstration  
**Version:** 1.0  
**Intended use:** evaluator training, QA calibration, rubric demonstration  
**Not intended for:** measuring or ranking commercial models, making claims about model performance, or serving as a validated research instrument.

## How to use

1. Read each task, reference material, and response under review.
2. Evaluate the response without assuming unstated facts.
3. Decompose it into material claims or requirements.
4. Classify evidence-dependent claims as **supported**, **contradicted**, or **not established**.
5. Score applicable dimensions using the parent [scoring rubric](../SCORING_RUBRIC.md).
6. Record evidence and a concise rationale.
7. Compare your result with the illustrative adjudication in [BENCHMARK_ANSWER_KEY.md](BENCHMARK_ANSWER_KEY.md).

For calibration exercises, evaluators should score cases independently before reading the answer key.

## Cases

| Case | Primary skill | Key risk |
|---|---|---|
| B-01 | Claim verification | Unsupported outcome inference |
| B-02 | Instruction adherence | Ignoring a hard format constraint |
| B-03 | Multilingual semantic QA | Changing modality and certainty in translation |

## Suggested calibration protocol

- Have at least two evaluators score each case independently.
- Compare dimension-level scores, not only the overall mean.
- Discuss disagreements using the task instructions and evidence.
- Record the agreed interpretation and any new precedent.
- Re-score the case after calibration to confirm consistent application.

A disagreement is not automatically an evaluator error. It may reveal an ambiguous rubric, incomplete evidence, or a need for domain expertise.

## Limitations

This is a deliberately small synthetic benchmark. It is useful for demonstrating a workflow, not for estimating inter-rater reliability or generalizing to model quality across domains. Expand the set and conduct a documented validation study before using it for consequential comparisons.
