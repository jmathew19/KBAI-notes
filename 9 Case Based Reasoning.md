# Case-Based Reasoning

## Introduction
Case-Based Reasoning (CBR) is a **problem-solving approach** where past experiences (cases) are adapted to solve new but similar problems. Unlike **learning by recording cases**, which retrieves identical cases, CBR involves **adapting** past cases to fit new situations.

CBR consists of **four main phases**:
1. **Case Retrieval** – Finding the most similar past case.
2. **Case Adaptation** – Tweaking the past solution to fit the new problem.
3. **Case Evaluation** – Assessing the adapted solution’s effectiveness.
4. **Case Storage** – Storing the new solution as a case for future use.

---

## Case-Based Reasoning vs. Learning by Recording Cases
### Example: Color Classification
- **Learning by Recording Cases**: Assigns the closest matching **color** to a new block.
- **CBR**: If no identical block exists, it **adapts** a past case (e.g., inferring a shade between two similar colors).
![[Screenshot 2025-02-22 at 2.13.01 PM.png]]
From [[8 Learn By Recording Cases]] we would say the block is orange, but in fact its pink
### Real-World Analogy
- **Navigation**:
  - **Learning by Recording Cases**: "Follow Route A, which worked before."
  - **CBR**: "Route D is close, let’s tweak the path."
![[Screenshot 2025-02-22 at 2.15.24 PM.png]]

- **Programming**:
  - Copying past **Java** code for file input and **modifying** it for **Python**.
- **Medical Diagnosis**:
  - A doctor adjusts a **previous diagnosis** for a new patient with similar but **not identical** symptoms.
- 

---

## The CBR Process
### 1. Case Retrieval
- Identify the **most similar** past case.
- **K-Nearest Neighbor (KNN)** is commonly used for retrieval.
- 

### 2. Case Adaptation
Once a case is retrieved, it **must be adjusted** to match the new problem.
Three methods for adaptation:
1. **Model-Based Adaptation**:![[Screenshot 2025-02-22 at 2.26.21 PM.png]]
   - Uses **a model of the world** to tweak past solutions.
   - Example: Adapting **a known driving route** using a map.


2. **Recursive Case-Based Adaptation**:![[Screenshot 2025-02-22 at 2.25.59 PM.png]]
   - Breaks the problem into **sub-problems** and solves them recursively.
   - Example: Breaking **a complex programming task** into smaller parts.

3. **Rule-Based Adaptation**:
   - Uses **heuristics** to guide adaptation. Rule of thumb but does not always hold truth
   - Example: "Reverse the steps of a known solution to go back."
    ![[Screenshot 2025-02-22 at 2.27.54 PM.png]]


### 3. Case Evaluation
- The adapted solution is **tested or simulated**.
- If it **fails**, the case is revised or another past case is retrieved.

### 4. Case Storage
- Successful solutions are **stored** for future use.
- Failed cases can also be stored to **anticipate future failures**.
- **Indexing**: 
	- Store data in coordinate structure![[Screenshot 2025-02-22 at 2.29.41 PM.png]]
	- Discrimination Trees![[Screenshot 2025-02-22 at 2.31.51 PM.png]]
---

## Organizing Case Memory
### Indexing Cases
- Cases are stored using **tags** (e.g., **file type, language, efficiency** in programming).
- Indexing allows **efficient retrieval**.

### Discrimination Trees
- A **decision tree** structure is used for **fast searching**.
- Instead of linear lookup, cases are **pruned** based on relevance.

---

## Strengths and Limitations
### Strengths:
✅ **Mimics human reasoning** – Adjusts past experiences instead of reinventing solutions.  
✅ **Efficient in structured domains** – Useful in law, medicine, engineering, and AI.  
✅ **Combines memory, reasoning, and learning** for adaptive intelligence.  

### Limitations:
❌ **Not always efficient** – Adapting cases can be complex.  
❌ **Requires good case storage** – Poor organization makes retrieval difficult.  
❌ **Similar problems can have different solutions** – Sometimes, past cases don’t generalize well.  

---

## Conclusion
CBR enhances **learning by recording cases** by adding **adaptation and evaluation**. It forms the **core of analogical reasoning**, making AI systems more **flexible** and **intelligent**.

Next steps in AI learning include **incremental concept learning**, which abstracts over cases to develop broader concepts.

