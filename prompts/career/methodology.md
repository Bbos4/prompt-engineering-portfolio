# Design Methodology: Concept Simplifier

## Design Goal
This prompt aims to help educators, students, and tutors break down academic or technical concepts into explanations using structured real-world analogies.

---

## Design Approach: Structure and Technique

**Structure I used:** Custom **C-A-R-E** structure (*Context, Action, Requirements, Example*).

**Why this structure fits my task:**
- **Context Necessary:** Defining the context for the AI sets the correct tone suitable for teaching.
- **Component connecting:** `Requirements` ensures the AI does not just tell a story, but connects each part of the analogy back to the real subject.

**Technique I used:** **Few-Shot Prompting**.

**Why this technique fits my task:**
I used few-shot prompting because because by providing a complete worked example showing a plain definition the model learns the exact depth, tone, and structural format required.

---

## Part-by-Part Justification

| Part | What I put here | Why the prompt needs it |
|------|-----------------|-------------------------|
| **[CONTEXT]** | Educator persona definition | Sets an accessible, clear, and encouraging tone suitable for teaching. |
| **[ACTION]** | Core task & audience placeholder | Captures the specific topic to explain and specifies the target audience level. |
| **[REQUIREMENTS]** | Formatting rules & constraint list | Mandates a short definition, mapping table, and banning jargon. |
| **[EXAMPLE]** | Worked API/Waiter analogy example | Demonstrates the expected structure, table layout, and tone. |

---

## Testing and Iteration

**Baseline I compared against:**
```Explain [TARGET_CONCEPT] to a [TARGET_AUDIENCE_LEVEL] using an analogy.```

| Version | Result / score | What changed |
|---------|----------------|--------------|
| Naive baseline | 35 / 100 | provided specifics and context but not outputs. |
| Version 1 | 78 / 100 | good overall but could have better framework and outputs. |
| Final |  / 100 | Added the mandatory table that compares the analogy directly to the concept. |

**What testing showed:** The prompt ran much better than the baseline, a much more specific output and answer.

**What I learned:** Giving examples for the AI to follow in the right situation can make or break the prompt.

---
## Strengths and Limitations
**Works well when:** Explaining abstract topics
**Struggles when:** When given something to explain without specific components or clear components so the analogies are difficult.
**Would improve next:** Have it explain the limits of the analogies.
