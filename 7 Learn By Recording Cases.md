# Learning by Recording Cases

## Introduction
Learning by recording cases is a **fundamental learning method** in knowledge-based AI. It is a key component of **analogical reasoning**, where past experiences are stored and reused to solve new problems.

This method involves:
1. **Recording cases** – Storing past experiences in memory.
2. **Retrieving cases** – Finding the most similar past case when faced with a new problem.
3. **Applying solutions** – Using the retrieved case to solve the new problem.

---

## How Learning by Recording Cases Works
### Example: Recognizing Block Colors
- Given six colored blocks, a new block is introduced.
- The AI **retrieves the most similar case** from memory.
- The AI assumes the new block has the **same color** as the closest matching case.
![[Screenshot 2025-02-21 at 2.30.07 PM.png]]
![[Screenshot 2025-02-21 at 2.31.10 PM.png]]
![[Screenshot 2025-02-21 at 2.32.10 PM.png]]

to find out we can do the distance formula and see that the black block is the closest option

## Nearest Neighbor Method
To retrieve the most similar case, AI calculates the **distance** between the new problem and past cases.

### **Euclidean Distance Formula**
The similarity between two cases is measured using:

\[d = \sqrt{(x_1 - x_2)^2 + (y_1 - y_2)^2}\]
### Real-World Analogy
- **Tying Shoelaces**: You don’t analyze the process each time—you recall a past successful experience.
- **Programming**:
  - When starting a new Java program, recall previous programs and use **public static void main**.
  - When encountering a **null pointer error**, recall a past case where debugging resolved the issue.
- **Medical Diagnosis**:
  - A doctor recalls past patient cases with similar symptoms to make a diagnosis.

---

## k-Nearest Neighbor (k-NN) Method
- Instead of selecting only **one** nearest case, AI considers **k** closest cases.
- The final decision is based on the majority of similar cases.
- **Example**: A self-driving car selects the best route by considering **multiple past successful routes**.

---

## Applications in AI
### **Navigation Systems**
- An autonomous car navigates based on **ONLY** stored routes.
- The AI retrieves past routes and selects the most similar path.

![[Screenshot 2025-02-21 at 2.35.13 PM.png]]

Looking at Q and the end we see (visually)that D is the most similar, but we need to design some computational way to decide it:


![[Screenshot 2025-02-21 at 2.39.26 PM.png]]
From here we can calc the nearest neighbor for all points, we see that d is the "shortest distanced" from them 

![[Screenshot 2025-02-21 at 2.40.15 PM.png]]

---

## Strengths and Limitations
### Strengths:
✅ **Simple and intuitive** – Mimics human memory-based problem-solving.  
✅ **Works well in structured domains** – Effective in medical diagnosis, navigation, and object recognition.  
✅ **No need for explicit rules** – The system learns directly from experience.  

### Limitations:
❌ **Curse of Dimensionality** – High-dimensional data makes similarity calculations difficult.  
❌ **Blind Application** – A past solution may not always be valid for a new problem.  
❌ **Memory-intensive** – Storing and retrieving large numbers of cases can be inefficient.  

---

## Conclusion
Learning by recording cases is a **powerful method** that shifts the balance from **reasoning** to **memory retrieval**. While effective in many situations, it has challenges that require enhancements like **case adaptation** and **case-based reasoning**.

The next step in AI learning is to **adapt** past cases rather than just reusing them—a concept explored in **case-based reasoning**.

