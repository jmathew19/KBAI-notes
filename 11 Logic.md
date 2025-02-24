# Logic

## Introduction
Logic is a **formal language** that allows us to make **precise assertions** about the world. It serves as the foundation for many AI applications, including **planning, reasoning, and knowledge representation**.

### Key Topics:
1. **Formal Notation** – Writing structured logical sentences.
2. **Truth Tables** – Evaluating logical expressions.
3. **Rules of Inference** – Modus Ponens, Modus Tollens.
4. **Proof Techniques** – Resolution theorem proving.
5. **Logic in AI Agents** – Knowledge bases and inference engines.

---

## Why Use Formal Logic in AI?
- **Two components** of a logic-based AI agent:
  1. **Knowledge Base (KB)** – Stores factual knowledge in logical sentences.
  2. **Inference Engine** – Applies rules of inference to draw conclusions.
- **Ensuring Correctness:**
  - **Soundness**: Only derives **valid** conclusions.
  - **Completeness**: Derives **all valid** conclusions.

---

## Logical Representation
### Example: Animal Classification
- A **classification hierarchy** can be expressed using logic.
- Example:
  - If an animal **has feathers**, then it is a **bird**:
    - \[ Feathers(animal) \Rightarrow Bird(animal) \]
  - If an animal **lays eggs** and **flies**, then it is a **bird**:
    - \[ LaysEggs(animal) \land Flies(animal) \Rightarrow Bird(animal) \]

---

## Logical Operators and Truth Tables
### Basic Logical Connectives:
| Operator   | Symbol                | Meaning                                |
| ---------- | --------------------- | -------------------------------------- |
| AND        | ∧                     | True if both statements are true       |
| OR         | ∨                     | True if at least one statement is true |
| NOT        | ¬                     | Negates the truth value                |
| IMPLIES    | ⇒                     | If A is true, then B must be true      |
| EQUIVALENT | \( \Leftrightarrow \) | A is true if and only if B is true     |

### Example: Truth Table for OR (\( \lor \))
| A   | B   | A ∨ B |
| --- | --- | ----- |
| T   | T   | T     |
| T   | F   | T     |
| F   | T   | T     |
| F   | F   | F     |

---
## Implication Elimination 

#### Given                            a ⇒ b
### Rewrite as:              ¬a ∨ b
----
## Rules of Inference
### 1. **Modus Ponens**
If \( p ⇒ q \) and \( p \) is true, then \( q \) is true.
- Example:
  - **If an animal has feathers, then it is a bird.**
  - **This animal has feathers.**
  - **Therefore, it is a bird.**

### 2. **Modus Tollens**
If \( p ⇒ q \) and \( q \) is false, then \( p \) must be false.
- Example:
  - **If an animal has feathers, then it is a bird.**
  - **This animal is NOT a bird.**
  - **Therefore, it does NOT have feathers.**
---

## Resolution Theorem Proving
Resolution theorem proving is a **more efficient** proof technique for logic.
### Steps:
1. Convert sentences into **Conjunctive Normal Form (CNF)**.
2. **Negate the goal** (proof by refutation).
3. Apply **resolution rule** to simplify.
4. If a **contradiction (null clause)** is reached, the proof is complete.
### Example:
![[Screenshot 2025-02-22 at 2.59.04 PM.png]]


---

## First-Order Logic (FOL)
- **Extends propositional logic** by introducing **quantifiers and variables**.
- Example:
  - **Universal Quantification (\( \forall \))**:
    - **All birds have feathers:**
      - \( \forall x (Bird(x) \Rightarrow Feathers(x)) \)
  - **Existential Quantification (\( \exists \))**:
    - **Some animals can fly:**
      - \( \exists x (Animal(x) \land Flies(x)) \)

---

## Logic in AI Applications
### 1. **Expert Systems**
- AI uses logic to **diagnose diseases** or **troubleshoot issues**.
- Example: **Medical Diagnosis**
  - \( \text{Fever} \land \text{Cough} \Rightarrow \text{Flu} \)

### 2. **Automated Theorem Proving**
- AI proves **mathematical theorems** using logic.

### 3. **Planning and Decision-Making**
- Logical inference helps AI **plan actions** and achieve **goals**.

---

## Strengths and Limitations of Logic in AI
### Strengths:
✅ **Provides formal correctness** in reasoning.  
✅ **Enables precise and explainable AI decisions.**  
✅ **Forms the foundation for many AI algorithms.**  

### Limitations:
❌ **Computationally expensive** – Large knowledge bases make inference slow.  
❌ **Requires complete and correct knowledge bases.**  
❌ **Struggles with uncertain or probabilistic reasoning.**  

---

## Conclusion
Logic is a **fundamental AI tool** for **knowledge representation and reasoning**. It helps build **intelligent agents** that can:
- **Store structured knowledge**.
- **Draw valid inferences**.
- **Prove facts efficiently**.

Next, we explore **planning**, which builds upon logical reasoning to help AI agents achieve goals systematically.

