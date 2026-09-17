# Design Methodology: Elevator Pitch Builder

## Design Goal
This prompt enables job seekers and professionals to quickly generate a clear, confident, elevator pitch.

---

## Design Approach: Structure and Technique

**Structure I used:** **R-T-F** structure.

**Why this structure fits my task:**
- **Role:** Setting an executive coach persona ensures the output sounds confident, polished, and professional.
- **Task:** Clear operational rules specify right peices.
- **Format:** Breaking the output into a script that uses all the pieces necessary

**Technique I used:** **Zero-Shot Prompting**.

**Why this technique fits my task:**
Zero-Shot prompting is good here because creating an elevator pitch uses personal details rather than pattern matching against an example. By using strict word count boundaries and direct constraints it produces a natural, ready-to-use script on the first attempt without needing an example.

---

## Part-by-Part Justification

| Part | What I put here | Why the prompt needs it |
|------|-----------------|-------------------------|
| **[ROLE]** | Executive coach & strategist | Directs the model toward persuasive communication principles. |
| **[TASK]** | User background inputs & strict constraints | Captures candidate data and enforcing strict word limits. |
| **[FORMAT]** | 4 part structured layout | creates a good and well formatted elevator pitch to grab attention and deliver. |

---

## Testing and Iteration

**Baseline I compared against:**
```Write an elevator pitch for me based on my experience: [BACKGROUND], [TARGET_ROLE].```
| Version | Result / score | What changed |
|---------|----------------|--------------|
| Naive baseline | 25 / 100 | provided specifics and context but not outputs. |
| Final | 100 / 100 | has all the necessary parts, specific, structured, Context, and Good output.|
**What testing showed:** The prompt ran much better than the baseline, a much more specific output and answer.

---
## Strengths and Limitations
**Works well when:** preparing for a interview
**Struggles when:** needing to be more unique as there arn't personal skills inputed
**Would improve next:** add a piece that talks about your specific skills.
