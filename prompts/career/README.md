# Concept Simplifier

A structured educational prompt that takes difficult, technical, or abstract concepts and breaks them down into explanations using clear, relatable real-world analogies.

- **Use case 1:** Explaining complex STEM concepts to students.
- **Use case 2:** Creating study guide summaries.

**Structure:** Custom C-A-R-E Structure (*Context, Action, Requirements, Example*).  
**Technique:** Few-Shot Prompting.  
**Output:** A structured Markdown summary containing a plain-English definition, and real-world analogy.

---

## Quick Start
1. Open [`prompt.md`](./prompt.md) and copy the template.
2. Replace the placeholders:
   - `[TARGET_CONCEPT]`: The difficult or abstract topic you want explained (e.g., *APIs*, *Quantum Entanglement*, *Inflation*).
   - `[TARGET_AUDIENCE_LEVEL]`: The intended reader (e.g., *Middle School Student*, *High School Senior*, *Non-technical Adult*).
3. Paste it into your AI model of choice and run it.
4. Review the output and adapt it to what you need.

---

## Examples
See the [`examples/`](./examples/) folder for filled-in demonstrations showing the prompt and the resulting output.

---

## Customization Tips
- **Want more detail?** Add an extra requirement under `[REQUIREMENTS]` asking the model to include misconceptions about the topic.
- **Want it shorter?** Request only the core analogy.
- **Different context?** Adjust `[CONTEXT]` like to explain something for a test.

---

## Technical Details
- **Structure:** Custom C-A-R-E (*Context, Action, Requirements, Example*)
- **Technique:** Few-Shot Prompting
- **Best models:** GPT-4o, Claude 3.5 Sonnet, Gemini 1.5 Pro
- **Placeholders:** 2 (`[TARGET_CONCEPT]`, `[TARGET_AUDIENCE_LEVEL]`)
