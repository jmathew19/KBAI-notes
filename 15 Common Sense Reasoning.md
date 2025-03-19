# Common Sense Reasoning - Lecture Notes

Video ID: rmby_NOApI4
### Introduction to Common Sense Reasoning
- Humans excel at common sense reasoning, making natural, obvious inferences.
- AI agents struggle with similar reasoning tasks.
- Example: A robot tasked with checking the weather outside shouldn't jump out of the window.
- The challenge: How can AI agents learn to make common sense inferences?

### [[7 Frames]] Representation
- AI can utilize a **frame representation** for reasoning.
- Introduces **primitive actions** (only 14), which:
  - Organize knowledge.
  - Form hierarchies of sub-actions.
  - Lead to changes in state, allowing inference.
- Helps AI predict potential outcomes of actions, preventing unreasonable decisions.

---

Video ID: N4aii1-WV3o
### Understanding Meaning in AI
- Machines struggle with **disambiguating meanings** of words.
- Example: The verb "eat" has multiple meanings:
  - **Physical consumption:** "Ashok ate a frog."
  - **Metaphorical usage:** "The river ate away at the riverbank."
- AI must use **sentence structure and background knowledge** to determine meaning.
- AI also faces challenges with **synonyms**:
  - "Ashok ingested a frog" vs. "Ashok devoured a frog" – same core meaning.
- **Context plays a crucial role** in determining meaning.

This is the inverse of the problem from [[14 Understanding]] where one word has multiple meanings, we now have multiple words for the same meaning. 

Context matters in helping understanding one word has multiple meanings, and multiple words for the same meaning
![[Screenshot 2025-03-05 at 11.56.35 AM.png]]

---

Video ID: gXU4RC6w-Mo
### Using Primitive Actions for AI Story Understanding
- **Primitive actions** help simplify AI interpretation of sentences.
- Example: "Ashok ate a frog" → maps to a **primitive action "ingest."**
- Key steps in AI understanding:
  1. Identify **agent** (Ashok).
  2. Identify **object** (frog).
  3. Recognize **state change** (frog moves from outside to inside Ashok).
- AI must extract **implicit knowledge** (e.g., Ashok is likely happy after eating the frog).
![[Screenshot 2025-03-05 at 11.59.20 AM.png]]
We can now apply the primitive to the sentences we had earlier
![[Screenshot 2025-03-05 at 12.02.21 PM.png]]

---

Video ID: YydQ_uPO2f0
### Identifying Primitive Actions
- AI must map verbs to primitive actions:
  - **John pushed the cart** → "propel" action.
  - **John took the book from Mary** → "transfer" action.
  - **John ate ice cream** → "ingest" action.
  - **John decided to go to the store** → Decision-making process.
- **Challenges:**
  - Some sentences contain multiple verbs.
  - Context determines the most appropriate primitive action.
![[Screenshot 2025-03-05 at 12.06.53 PM.png]]
---

Video ID: IdpWlJskfNo
### AI Processing Steps
- AI **reads left to right** in English.
- Steps for understanding "John pushed the cart":
  1. Identify **subject (John)**.
  2. Identify **verb (pushed)**.
  3. Retrieve **frame for "propel"** from memory.
  4. Assign **agent (John)** and **object (cart)** to frame slots.
- AI uses **bottom-up (data-driven) and top-down (knowledge-driven) processing**.
- Primitive actions **act as hooks** to pull relevant meanings.
![[Screenshot 2025-03-05 at 12.08.30 PM.png]]

---
## Implied Action 

take sentence: **"John fertilizer of the field"**
we know that it can be rewritten as **"John PUT fertilizer of the field"**

The AI needs to understand implied action to make it transparent so that it can apply primitive actions 

The sentence is difficult to map out the primitive action so we need to 

Bill fired a bullet at Bob. → Bill propelled a bullet into Bob.

We can easily map it out now
![[Screenshot 2025-03-05 at 12.18.53 PM.png]]



---

Video ID: HIHT6Wmzcyw
### Handling Ambiguous Sentences
- Example: "Bill shot Bob."
  - Possible meanings:
    1. Bill fired a bullet at Bob. → Bill propelled a bullet into Bob.
    2. Bill took a picture of Bob.
  - AI must **use context** to disambiguate.
- AI **may revise interpretations** if it realizes the initial frame does not fit.

---

Video ID: 1Yj-Js33V6A
### Common Sense Reasoning in AI
- AI needs **background knowledge** to make inferences.
- Example: "Ashok put the wedge on the block."
  - AI should infer that **Ashok’s hand moved**, even if not stated explicitly.
  - **Micro-stories** provide sub-actions (grasping, moving, releasing).

![[Screenshot 2025-03-05 at 12.20.29 PM.png]]
---

Video ID: eVqJy614AvU
### Applying Common Sense Reasoning to AI Challenges
- Could AI use these techniques to solve **Raven’s Progressive Matrices**?
- **Primitive actions** could correspond to **visual transformations**.
- AI could recognize **patterns** and **higher-level transformations**.
![[Screenshot 2025-03-05 at 12.23.05 PM.png]]
---

Video ID: Ol9q0kSyGtc
### Susan comforted Jing
-  ![[Screenshot 2025-03-05 at 12.24.35 PM.png]]

![[Screenshot 2025-03-05 at 12.25.35 PM.png]]
---

Video ID: XjmXo3vrnk4
### Connection to Human Cognition
- Humans **use context** to decide on appropriate actions.
- AI must **model "Theory of Mind"**:
  - Assigning **goals, beliefs, and desires** to others.
  - Helps in **social common sense reasoning**.

---
