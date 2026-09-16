# Customer Reviewer & Feedback Advice
> *A structured business prompt designed to turn messy, unstructured customer feedback into actionable product insights, and a strategic course of action.*
**Best for:**
- Use case 1: Extracting operational strengths and weaknesses from unorganized customer review text.
- Use case 2: Identifying high risks and product issues early.
- Use case 3: Formulating a strategic course of action to address and resolve top customer concerns.

**Structure:** Custom S-A-F-E Structure (*Situation, Analysis, Findings, Execution*).  
**Technique:** Zero-Shot Chain-of-Thought.  
**Output:** A structured Markdown report with step-by-step analytical reasoning and categorized bulleted findings.

---

## Quick Start
1. Open [`prompt.md`](./prompt.md) and copy the template.
2. Replace the placeholders:
   - `[COMPANY_TYPE_AND_PRODUCT]`: The type of business and primary good or service.
   - `[RAW_CUSTOMER_REVIEWS]`: Unedited customer reviews or support tickets.
3. Paste it into your AI model of choice and run it.
4. Review the output and adapt it to what you need.

---

## Examples
See the [`examples/`](./examples/) folder for filled-in demonstrations showing the prompt and the resulting output.

---

## Customization Tips
- **Want more detail?** Add an extra instruction under `[ANALYSIS]`
- **Want it shorter?** Remove the `[EXECUTION]` section if you only need to know the issues.
- **Different context?** Change `[SITUATION]` to an app review or whatever context needed otherwise.

---

## Technical Details
- **Structure:** Custom S-A-F-E (*Situation, Analysis, Findings, Execution*)
- **Technique:** Zero-Shot Chain-of-Thought (Zero-Shot CoT)
- **Best models:** GPT-4o, Claude 3.5 Sonnet, Gemini 1.5 Pro
- **Placeholders:** 2 (`[COMPANY_TYPE_AND_PRODUCT]`, `[RAW_CUSTOMER_REVIEWS]`)
