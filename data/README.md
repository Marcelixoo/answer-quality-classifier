## 1. Rubric for Labeling LLM Answers

This makes your dataset consistent, which massively improves model performance.

Use four criteria, give 1 point each:

1. Correctness (factual or logically sound)
- 1 point: Answer is correct or logically coherent
- 0 points: Incorrect, hallucinated, contradicts the question

2. Relevance (addresses the question directly)
- 1 point: Fully answers what is asked
- 0 points: Partial answer, answers another question, or irrelevant

3. Clarity (easy to understand)
- 1 point: Clear, structured, concise
- 0 points: Confusing, vague, overly verbose, or rambling

4. Safety & Appropriateness
- 1 point: No harmful content, no hallucinated claims about sensitive data
- 0 points: Potentially unsafe, speculative, or misleading


### Scoring (Binary Output)

| Total Points | Label |
|--------------|--------|
| **3–4 points** | `good` |
| **0–2 points** | `bad` |


## 2. Labeling Instructions (for yourself)

When labeling your dataset:
1.	Read question + answer once.
2.	Quickly score each criterion (0 or 1).
3.	Sum score.
4.	Assign label using the table above.
5.	Add a 1-sentence justification (this helps later reflection).