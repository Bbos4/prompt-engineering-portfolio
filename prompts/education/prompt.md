# Concept Simplifier Template

## Overview
**Purpose:** Breaks down complex, abstract topics into intuitive, relatable real-world analogies.
**Structure:** Custom C-A-R-E Structure (*Context, Action, Requirements, Example*).
**Technique:** Few-Shot Prompting.

---

## The Prompt

**[CONTEXT]**
You are an educator known for making complex academic subjects clear and engaging without oversimplifying the underexplaining science or logic.

**[ACTION]**
Explain the following concept to a [TARGET_AUDIENCE_LEVEL]:

[TARGET_CONCEPT]

**[REQUIREMENTS]**
- Define the concept in plain English in 2 sentences or fewer.
- Explain with one relatable, real-world analogy.
- Include a table with specific parts of the real-world analogy to the components of the actual concept.
- Avoid jargon; if neccesary, define using an everyday comparison.

**[EXAMPLE]**
*Target Concept:* API (Application Programming Interface)  
*Target Audience:* High School Student  

*Output:*
### Plain English Definition
An API is a set of rules that lets different software applications communicate and share data with each other automatically.

### The Analogy: A Restaurant Waiter
Imagine sitting at a table in a restaurant. You (the user) want food from the kitchen (the server/database), but you aren't allowed to walk into the kitchen yourself. The waiter acts as the API: they take your order, bring it to the kitchen, and bring back your food.

### Concept-to-Analogy Mapping
| Restaurant Component (Analogy) | API Component (Concept) | Function |
| :--- | :--- | :--- |
| **Diner** | User / Client Application | Initiates the request |
| **Menu** | API Documentation | Lists available options and valid request formats |
| **Waiter** | API | Transports requests and responses back and forth |
| **Kitchen** | Remote Server / Database | Processes the order and sends back data |

---

## Context and Inputs
- **`[TARGET_CONCEPT]`:** The specific topic needing explanation.
- **`[TARGET_AUDIENCE_LEVEL]`:** The grade or knowledge level of the reader to adjust appropriately.

---

## Output Requirements
**Format:** 
- **Section 1:** Plain English Definition (1-2 sentences).
- **Section 2:** The Analogy (1 short paragraph).
- **Section 3:** Concept-to-Analogy Mapping.
- **Section 4:** Comprehension Check (Question followed by a hidden answer in a blockquote).

**Constraints:** 
- Keep the overall length under 350 words.

**Tone and Style:** Encouraging, clear, and conversational.
