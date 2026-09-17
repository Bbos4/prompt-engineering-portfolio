# Customer Reviewer & Feedback Advice

## Overview
**Purpose:** Analyzes unorganized customer reviews to extract key sentiment drivers, and establish a clear course of action for resolving top concerns.
**Structure:** Custom S-A-F-E Structure (*Situation, Analysis, Findings, Execution*).
**Technique:** Zero-Shot Chain-of-Thought (Zero-Shot CoT).

---

## The Prompt

**[SITUATION]**
You are a Lead Customer support worker for [COMPANY_TYPE_AND_PRODUCT]. You have been provided with unedited customer reviews:

[RAW_CUSTOMER_REVIEWS]

**[ANALYSIS]**
Think through this step-by-step before producing your final report:
1. Examine each review individually and identify weather it is Positive, Neutral, or Negative.
2. Group common feedback patterns into clear operational themes.
3. Isolate high-severity issues—identify specifically which negative points create immediate leaving risks or refund requests.

**[FINDINGS]**
Summarize your analysis into three distinct sections:
- **Top 3 Strengths:** What customers love most about the product or service.
- **Top 3 Friction Points:** Critical points causing customer frustration or customers leaving.
- **Feature & Improvement Wishlist:** Suggestions mentioned or implied by users.

**[EXECUTION]**
Provide a prioritized, step-by-step course of action explaining how management should address and resolve the biggest concerns identified in the analysis.

---

## Context and Inputs
- **`[COMPANY_TYPE_AND_PRODUCT]`:** Defines the business context so the model understands industry norms, product types, and customer expectations.
- **`[RAW_CUSTOMER_REVIEWS]`:** The raw text dataset containing customer reviews or support tickets for the model to analyze.

---

## Output Requirements
**Format:** 
- **Section 1:** Step-by-Step Reasoning.
- **Section 2:** Markdown Bulleted Lists for Findings.
- **Section 3:** Numbered List outlining a strategic Course of Action for management.

**Constraints:** 
- Do not make up customer sentiments or issues that are not supported by the reviews.
- Focus course of action steps on root operational fixes rather than surface-level workarounds.
- Keep recommendations actionable and realistic for a business to implement.

**Tone and Style:** Analytical, strategic, and professional.
