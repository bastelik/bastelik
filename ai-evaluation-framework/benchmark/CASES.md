# Benchmark Cases

All scenarios and source excerpts below are fictional and created solely for evaluator practice.

## B-01 — Unsupported outcome inference

**Primary dimensions:** factual accuracy, evidence handling, instruction adherence.

### Task

Summarize the supplied report excerpt in no more than two sentences. Do not infer outcomes that the report did not measure.

### Reference excerpt

"The 2025 pilot enrolled 180 participants across three locations. The evaluation tracked attendance and completion. It did not collect data on participants' income or employment after the program."

### Response under review

"The 2025 pilot enrolled 180 participants at three locations and improved their employment prospects."

### Evaluator prompts

- Separate the enrollment and location claims from the employment claim.
- Does the excerpt establish an improvement in employment prospects?
- Did the response comply with the explicit instruction?

---

## B-02 — Failure to follow a hard format constraint

**Primary dimensions:** instruction adherence, completeness, communication.

### Task

Return exactly three bullet points. Each bullet must contain one action verb and no more than eight words. Use only the following source facts:
- The team will review terminology on Monday.
- The project lead will send the revised schedule on Tuesday.
- Quality assurance will report unresolved issues on Wednesday.

### Response under review

"Here is the plan:
- Review terminology with the team on Monday.
- The project lead will send the revised schedule on Tuesday.
- QA will report unresolved issues on Wednesday.
- Let me know if you need anything else."

### Evaluator prompts

- Count the bullets.
- Check the word count of each bullet.
- Identify whether the response adds material outside the requested format.
- Do not give full credit merely because the facts are accurate.

---

## B-03 — Modality shift in multilingual QA

**Primary dimensions:** factual accuracy, language quality, evidence handling.

### Task

Translate the following Portuguese sentence into English, preserving its level of certainty:

"Os resultados podem indicar uma melhora, mas ainda não permitem confirmar uma relação causal."

### Reference meaning

The results may indicate an improvement, but they do not yet allow a causal relationship to be confirmed.

### Response under review

"The results demonstrate an improvement and confirm a causal relationship."

### Evaluator prompts

- Compare "podem indicar" with "demonstrate."
- Compare "não permitem confirmar" with "confirm."
- Identify whether the translation preserves uncertainty and negation.
- Explain why fluent English is not sufficient for a high-quality translation.
