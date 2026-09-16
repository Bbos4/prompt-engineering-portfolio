# Design Methodology: Customer Review & Sentiment Analyzer

## Design Goal
This prompt aims to transform unstructured customer review text into actionable business intelligence, categorized risk reports, and a strategic course of action for business owners and customer experience leads.

---

## Design Approach: Structure and Technique

**Structure I used:** Custom **S-A-F-E** structure (*Situation, Analysis, Findings, Execution*).

**Why this structure fits my task:**
- **Logical Flow:** It moves the model naturally from receiving raw context (`Situation`), to reasoning through data (`Analysis`), categorizing outputs (`Findings`), and establishing solutions (`Execution`).
- **Action-Oriented End Goal:** Transitioning from passive analytical findings to an active course of action ensures the output gives management immediate steps to take rather than just raw data.

**Technique I used:** **Zero-Shot Chain-of-Thought (Zero-Shot CoT)**.

**Why this technique fits my task:**
I used zero-shot chain-of-thought because customer feedback varies wildly in tone, length, and topic, making fixed examples hard to standardize. Adding the instruction *"Think through this step-by-step before producing your final report"* forces the model to evaluate underlying sentiment and group operational themes logically before jumping to conclusions.

**Example of modifying a framework:**
I started from C-A-R-E (Context, Action, Result, Example) and adapted it into S-A-F-E (Situation, Analysis, Findings, Execution). I replaced Example with **Analysis** to force a chain-of-thought step, and changed Result to **Execution** to focus on a strategic course of action. This custom alignment fit a business analysis task far better than standard creative frameworks.

---

## Part-by-Part Justification

| Part | What I put here | Why the prompt needs it |
|------|-----------------|-------------------------|
| **[SITUATION]** | Role definition & business context placeholder | Establishes the business domain and provides the input dataset space so the AI understands industry expectations. |
| **[ANALYSIS]** | Explicit step-by-step reasoning instructions | Enforces Zero-Shot Chain-of-Thought logic, forcing the AI to evaluate individual reviews before categorizing them. |
| **[FINDINGS]** | Structured reporting sections (Strengths, Risks, Wishlist) | Ensures scannable, standardized output that business leads can review quickly. |
| **[EXECUTION]** | Step-by-step course of action plan | Converts analytical insights into a concrete operational playbook for addressing key concerns. |

---

## Testing and Iteration

**Baseline I compared against:**
```Read these reviews and tell me what customers think and how to fix negative ones: [RAW_REVIEWS]```
| Version | Result / score | What changed |
|---------|----------------|--------------|
| Naive baseline | 15 / 100 |  |
| Version 1 |  / 100 |  |
| Final |  / 100 | |
