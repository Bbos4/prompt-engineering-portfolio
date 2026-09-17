# Elevator Pitch Builder

A career prompt that uses a job seeker's background and target goal to generate a 30-second elevator pitch for networking interview intros.

- **Use case 1:** Answering tell me about yourself question in job interviews.
- **Use case 2:** Delivering an introduction at networking events.

**Structure:** R-T-F Structure
**Technique:** Zero-Shot Prompting.  
**Output:** A report containing a 30 second primary pitch.

---

## Quick Start
1. Open [`prompt.md`](./prompt.md) and copy the template.
2. Replace the placeholders:
   - `[CURRENT_ROLE_OR_BACKGROUND]`: Your current job title, field, or primary domain of experience.
   - `[TARGET_ROLE_OR_GOAL]`: The job, industry, or outcome you are aiming for next.
3. Paste it into your AI model of choice and run it.
4. Practice reading the output aloud to refine your natural speaking cadence.

---

## Examples
See the [`examples/`](./examples/) folder for filled-in demonstrations showing the prompt and the resulting output.

---

## Customization Tips
- **Want a specific tone?** Add a constraint specifying the setting and what the .
- **Changing careers?** you can add a sentance in task to explain how `[CURRENT_ROLE_OR_BACKGROUND]` can transition into `[TARGET_ROLE_OR_GOAL]`.

---

## Technical Details
- **Structure:** R-T-F
- **Technique:** Zero-Shot
- **Best models:** GPT-4o, Claude 3.5 Sonnet, Gemini 1.5 Pro
- **Placeholders:** (`[CURRENT_ROLE_OR_BACKGROUND]`, `[TARGET_ROLE_OR_GOAL]`)
