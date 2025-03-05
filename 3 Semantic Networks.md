# Semantic Networks

## Introduction
Semantic networks are a type of knowledge representation used in AI and cognitive science. This lesson explores how they represent relationships between concepts and how they enable problem-solving.

---

## Knowledge Representation
### Definition
- A **knowledge representation** consists of:
- A **language** with a defined vocabulary.
- **Content** that conveys meaningful information.

### Example:
- Newton’s second law: `F = ma`
  - **Language**: Algebraic equations (symbols and relationships)
  - **Content**: The principle of force, mass, and acceleration.

---

## Understanding Semantic Networks
### Conceptual Breakdown
1. **Objects Representation**
   - Each object is represented as a **node**.
   - Example: `x` (circle), `y` (diamond), `z` (black dot).

2. **Relationships Representation**
   - Links between nodes define relationships.
   - Example:
     - `y is inside x`
     - `z is above y`
     - `z is above x`

3. **Transformation Representation**
   - Links between different states capture changes.
   - Example: `x remains unchanged`, `y expands`, `z disappears`.

---

## Problem-Solving with Semantic Networks
### Example: 

![[Pasted image 20250220183714.png]]

![[Pasted image 20250220183756.png]]
---

## Characteristics of a Good Knowledge Representation
1. **Makes relationships explicit** – Clear object and relationship mapping.
2. **Right level of abstraction** – Captures essential details without redundancy.
3. **Concise & Transparent** – Focuses on relevant information.
4. **Computable** – Enables inference and reasoning.

---

## Real-World Example: Nutritional Labels
- Strengths:
  - Explicit values for each nutrient.
  - Helps users make dietary decisions.
- Limitations:
  - Doesn’t show relationships (e.g., how fat relates to calories).
  - Includes extraneous information for some users.

---

## Application: Guards and Prisoners Problem
- **Scenario:** Move three guards and three prisoners across a river.
- **Constraints:**
  - Prisoners must never outnumber guards on either side.
  - Boat can only carry up to two people.
- **Semantic Network Approach:**
  - Nodes represent different states.
  - Links capture legal and productive moves.
  - Illegal/unproductive moves are identified and removed.
![[Pasted image 20250221124816.png]]

---

## AI and Knowledge Representation
- **Inference Methods:** AI can evaluate transformation similarity.
- **Example:** Raven’s Progressive Matrices
  - Use semantic networks to represent and solve visual analogy problems.
- **Key Focus in AI:** Relationships over object properties.

---

## Assignment Idea
- Design a semantic network for **Raven’s Progressive Matrices**.
- Define:
  - Representation scheme.
  - How it supports problem-solving.
  - Its completeness and abstraction level.
- Compare different representations and their effectiveness.

---

## Conclusion
Semantic networks play a crucial role in knowledge representation and AI problem-solving. They make relationships explicit, support reasoning, and enable efficient decision-making.

