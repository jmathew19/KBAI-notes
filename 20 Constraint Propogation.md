# Lecture 20: Constraint Propagation in AI

Video ID: TGmEVlPIwsY
### Introduction to Constraint Propagation
- **Definition**:
  - **Method of inference** where AI assigns values to variables **to satisfy constraints**.
  - Used in **planning, language understanding, visual reasoning, and spatial reasoning**.
- **Topics Covered**:
  1. **Fundamentals of Constraint Propagation**.
  2. **Applications in Natural Language and Visual Processing**.
  3. **Advanced Issues in Constraint Propagation**.

Video ID: 9TJcNzFIT8Y
### Recognizing 3D Objects from 2D Images
- **Example**: Recognizing a cube drawn on a 2D surface.
- **Key Concepts**:
  - **Trihedral Objects**: Objects with three surfaces meeting at a point.
  - **Polyhedral Surfaces**: Multiple surfaces joining at one point (e.g., pyramids).
- **Ambiguity in Perception**:
  - Some figures have **multiple 3D interpretations**.
  - **Example**: A drawing may be seen as **looking into a box or viewing a building**.
![[Screenshot 2025-03-19 at 10.10.28 AM.png]]


Video ID: tgoSiW4lyQ8
### Detecting Grammar in Nonsensical Sentences
- **Example**: Identifying which sentences are grammatically correct.
- **Famous Sentence**: *"Colorless green ideas sleep furiously."*
  - **Semantically meaningless**, but **grammatically correct**.
- **Constraint-Based Language Processing**:
  - **Grammar imposes rules** that must be satisfied.
  - Words are assigned **parts of speech** (noun, verb, adjective, etc.).
  - Sentences must follow **syntactic constraints**.
![[Screenshot 2025-03-19 at 10.12.45 AM.png]]


Video ID: vQ7ucWQOQ4s
### Defining Constraint Propagation
- **Key Idea**:
  - Assigning values to **problem variables** while ensuring **global constraints** are met.
  - given variable assigned by task so that golbal constraints are satisfied
  - A problem is characterized by a certain variables 
  - How can we locally assign variables in such a way that global constraints are satisfied 
- **Example Applications**:
  - **Visual Processing**:
	  - ![[Screenshot 2025-03-19 at 10.17.26 AM.png]]
    - Determining if a **2D drawing represents a 3D object**.
    - Surfaces and orientations must **satisfy trihedral constraints**.
  - **Language Processing**:
	  - ![[Screenshot 2025-03-19 at 10.17.55 AM.png]]
    - Assigning words their **grammatical roles** while following English grammar.
    - Find what part of speech the word is?
    - 

Video ID: NIoy8ecK9d0
### Constraint Propagation in Computer Vision
![[Screenshot 2025-03-19 at 10.19.39 AM.png]]
- **Object Recognition Process**:
  1. **Detect edges and lines**.
  2. **Group lines into surfaces**.![[Screenshot 2025-03-19 at 10.20.25 AM.png]]
  3. **Assign orientations to surfaces**.![[Screenshot 2025-03-19 at 10.20.46 AM.png]]
  4. **Identify complete 3D objects**.
- **Lessons from AI & Computer Vision**:
  - **Task decomposition** helps break complex problems into sub-problems.

Video ID: UyjCINwZzII
### Line Labeling in Visual Perception
- **Defining the Problem**:
  - Look at sub task of grouping **lines into surfaces** using constraints.
  - **Surfaces must meet at specific angles** to form a 3D object.
  - ![[Screenshot 2025-03-19 at 10.20.25 AM.png]]
- **Types of Junctions**:
  - **Y-junctions**: Three lines meet.
  - **T-junctions**: One line is occluded.
  - **L-junctions**: Two surfaces meet at a right angle.
  - **W-junctions**: Complex surface intersections.

Video ID: eNokNL3hkoE
### Identifying Junction Types
- **Exercise**: Classify junctions in a cube.
- **Junction Types**:
  - **L, W, Y, and T junctions** exist in real-world objects.![[Screenshot 2025-03-19 at 10.25.34 AM.png]]
- **Key Insights**:
  - Each junction **follows specific constraints**.
  - Constraint propagation **refines interpretations**.
![[Screenshot 2025-03-19 at 10.30.49 AM.png]]

Video ID: W8vw7xh4Ofc
### Propagating Constraints to Detect Surfaces
- **Step-by-Step Process**:![[Screenshot 2025-03-19 at 10.31.07 AM.png]]
  1. **Identify junctions** in a 2D drawing.
  2. **Classify edges as folds or blades**.
  3. **Determine surfaces based on constraints**.
- **Outcome**:
  - Correctly **interpreting 2D images as 3D objects**.

Video ID: vM1lDp0oTPM
### Constraint Propagation in Language Processing
- **Example**: Parsing the sentence *"Colorless green ideas sleep furiously."*
- **Mini-Grammar Rules**:
  - A **sentence** consists of a **noun phrase + verb phrase**.
  - A **noun phrase** consists of **optional adjectives + noun**.
  - A **verb phrase** consists of **verb + optional adverb**.
- **Parsing Process**:
  - Assign **words their lexical categories**.
  - **Verify constraints** imposed by grammar rules.
  - **Confirm grammatical correctness**.

Video ID: CSoWol_KDpY
### Applying Constraint Propagation to Raven’s Progressive Matrices
- **Challenges in AI**:
  - Solving Raven’s matrices **without pre-defined rules**.
  - **Using primitive constraints** to understand visual reasoning.
- **Future Applications**:
  - Constraint propagation **could assist in AI-driven problem-solving**.

Video ID: ZChW12mHHqk
### Summary: The Role of Constraint Propagation in AI
- **Key Takeaways**:
  - Constraint propagation **assigns values to variables** while maintaining **global consistency**.
  - **Used in multiple AI areas**:
    - **Visual Processing**: Recognizing objects from images.
    - **Natural Language**: Understanding sentence structures.
  - **Future Applications**:
    - **Auditory Processing**.
    - **Tactile Perception** (e.g., reading Braille).
- **Next Topic**:
  - **Configuration Problems & Constraint-Based Design**.

---

[Download Lecture Notes](sandbox:/mnt/data/Lecture_20_Constraint_Propagation.md)

---

Let me know if you need modifications! 🚀
