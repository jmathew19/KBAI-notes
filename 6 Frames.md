# Frames

## Introduction
Frames are a **knowledge representation** technique that organizes information into structured templates. They consist of:
- **Slots**: Variables that store specific attributes.
- **Fillers**: Values assigned to slots.
- **Default Values**: Predefined assumptions that can be overridden.

Frames help in **common-sense reasoning** and allow AI systems to understand language, relationships, and actions.

---

## Properties of Frames
### 1. Stereotypes
- Frames represent **stereotypical** knowledge.
- Example: A frame for **"Ate"** includes slots for:
  - Subject: Who ate?
  - Object: What was eaten?
  - Location: Where did the eating happen?
  - Time: When did it happen?

![[Screenshot 2025-02-21 at 2.17.27 PM.png]]


### 2. Default Values
- Some slots have **default values**
- can be **Overridden**
- Example:
  - If "Ashok ate a frog," we assume:
    - The frog is **dead** (default assumption).
    - The frog is **inside Ashok’s stomach**.
    - Ashok is **happy** (unless stated otherwise).
![[Screenshot 2025-02-21 at 2.17.52 PM.png]]
### 3. Inheritance
- Frames **inherit** properties from parent frames.
- Example:
  - **Animal Frame** → General properties (e.g., has a body).
  - **Human Frame** (inherits from Animal) → More specific properties (e.g., has a job).
  - **Instance Frame** (e.g., "Ashok") → Personalized details.

![[Screenshot 2025-02-21 at 2.18.54 PM.png]]

![[Screenshot 2025-02-21 at 2.19.34 PM.png]]




---
![[Screenshot 2025-02-21 at 2.13.42 PM.png]]
## Connecting Frames
Frames can **link to other frames**:
- Example:
  - "Angela ate lasagna at Olive Garden with her dad."
  - A **Frame for Angela** can store:
    - Food preferences: Italian
  - A **Frame for Olive Garden** can store:
    - Location: Atlanta
  - A **Frame for Ate** connects these frames.

This enables **discourse-level understanding**, beyond individual sentences.
![[Screenshot 2025-02-21 at 2.15.06 PM.png]]
---

## Frames in AI and Natural Language Processing



### **Sentence Comprehension and Generation**
- Frames can act as an **intermediate representation**.
- **Example**:
  - Sentence: "Haruto ate sushi."
  - Frame Representation:
    - Subject: Haruto
    - Object: Sushi
    - Verb: Ate
  - This frame can be **reconstructed** into a sentence for generation.
![[Pasted image 20250221142125.png]]
### **Raven’s Progressive Matrices**
- Frames help represent **visual relationships**.
- Example:
  - A frame for **Object X** stores:
    - Shape: Triangle
    - Size: Large
    - Fill: Not filled
  - Frames capture **relationships** (e.g., "Object Y is inside Object X").

![[Screenshot 2025-02-21 at 2.23.07 PM.png]]

---

## Strengths and Limitations
### Strengths:
✅ **Encodes structured knowledge** in an intuitive way.  
✅ **Supports default values and exceptions** for flexibility.  
✅ **Links multiple frames** for complex reasoning.  
✅ **Combines top-down and bottom-up processing** for comprehension.  

### Limitations:
❌ **Handling exceptions is complex** (too many overrides can break structure).  
❌ **Cannot resolve ambiguities** (e.g., "Sadie Hawkins" as a **person** vs. **fault line**).  
❌ **Lacks deep reasoning capabilities** beyond predefined structures.  

---

## Conclusion
Frames are a **powerful** way to represent **conceptual knowledge** in AI. They enable:
- **Language understanding**
- **Problem-solving in AI**
- **Knowledge organization and inheritance**

While they have limitations, they remain a key tool in **cognitive systems and AI research**.

