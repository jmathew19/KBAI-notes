# Lecture 17: Explanation-Based Learning in AI

## Video ID: n8KQOsYms1Q
### Introduction to Explanation-Based Learning (EBL)
- **EBL Overview**:
  - The agent **does not learn new concepts**.
  - Instead, it **learns connections** among existing concepts.
- **Key Goals**:
  - Understanding **transfer of knowledge** from old to new situations.
  - Preparing for **analogical reasoning** in future discussions.
- **Topics Covered**:
  - **Concept Space**: Mapping relationships between concepts.
  - **Abstraction**: Generalizing knowledge for transfer.
  - **Transfer**: Applying previous knowledge to new problems.

## Video ID: j5YxvMvCYhc
### Soup Transportation Problem
- **Scenario**:
  - You need to transport soup, but **usual utensils are unavailable**.
  - Available objects: **Backpack, pitcher, box, car**.
  - **Which object do you use?** → **The pitcher**.
- **Human vs. AI Challenges**:
  - Humans find the solution **intuitive**.
  - AI must **explicitly reason through constraints**.
- **Connection to AI Learning**:
  - **Incremental Learning**: Learning from a small number of examples.
  - **Creativity in AI**: AI must generate novel solutions.

## Video ID: 4j_OryTZIAE
### AI Struggles with Simple Decisions
- **Why is this problem hard for AI?**
  - AI needs **structured reasoning** to determine why **a pitcher** is better than **a backpack**.
- **Comparison to Machine Learning**:
  - Unlike data-driven ML methods, **EBL learns incrementally**.
  - AI **derives knowledge from reasoning**, rather than detecting statistical patterns.

## Video ID: jHEZwUlRWR0
### Recognizing a Cup: A Creative Robot
- **Scenario**:
  - A household **robot makes coffee** and brings it in a cup.
  - One day, **no clean cups are available**.
  - The robot finds an **unknown object** and **evaluates if it can be used as a cup**.
- **AI’s Challenge**:
  - How does the robot **prove** the object is a cup?
  - AI must **build an explanation** to justify its reasoning.

## Video ID: T3pfV2GSVGU
### How AI Builds Explanations
- **Defining the Problem**:
  - AI must **prove** that an object is a cup.
  - AI has **knowledge about objects** (e.g., **shape, material, properties**).
- **Knowledge Representation**:
  - The AI must connect **observable facts** (e.g., concave shape) to **functional use** (e.g., holding liquid).

## Video ID: u6OU9q-3lpk
### Causal Knowledge in AI
- **AI Knowledge Base**:
  - **Brick**: Stable **because** it has a flat bottom.
  - **Briefcase**: Liftable **because** it is light and has a handle.
  - **Bowl**: Carries liquid **because** it is concave.
  - **Glass**: Enables drinking **because** it carries liquid and is liftable.
- **Key Insight**:
  - AI must **reason causally**, not just store facts.

## Video ID: uym1sxtq8Lw
### How AI Abstracts Knowledge
- **Example**: Generalizing from a bowl
  - AI **extracts only the causally relevant features**.
  - "A bowl carries liquid **because** it is concave" → Generalized as:
    - **"An object carries liquid because it is concave."**
- **Importance of Abstraction**:
  - AI **ignores irrelevant features**.
  - Focuses on **causally meaningful explanations**.

## Video ID: yRDp2Gd0Shw
### Constructing an Explanation: Proving an Object is a Cup
- **Step-by-step Explanation**:
  - AI **chains multiple abstractions**:
    1. Object is stable → **From the brick**.
    2. Object carries liquid → **From the bowl**.
    3. Object is liftable → **From the briefcase**.
    4. Object enables drinking → **From the glass**.
  - **Backward reasoning**:
    - AI **starts from the goal** ("Prove it’s a cup").
    - **Breaks it into subgoals** ("Prove it enables drinking").
    - **Selects supporting evidence from memory**.

## Video ID: IDfj-U7jdFA
### Exercise: Proving an Object is a Mug
- **Definition of a Mug**:
  - Stable.
  - Enables drinking.
  - **Protects against heat** (*New requirement*).
- **Challenge**:
  - AI must **prove heat protection**.
  - AI knows about a **pot**, which:
    - **Limits heat transfer** because it has **thick sides** and is **made of clay**.
  - **Failure to Complete Proof**:
    - AI **cannot link "limits heat transfer" to "protects against heat."**
    - The missing connection prevents a complete proof.

## Video ID: CooyadGqzbk
### Finding Missing Knowledge
- **AI needs minimal, relevant knowledge**.
- **Two approaches**:
  1. **Expand background knowledge** (e.g., add information about insulation).
  2. **Opportunistic reasoning** (use the best available knowledge).

## Video ID: 3hfSjxV4fgo
### Everyday Improvisation and EBL
- **Real-world examples**:
  - Using a **mug** as a **paperweight**.
  - Using a **chair** as a **doorstop**.
- **EBL in Human Reasoning**:
  - Humans **repurpose objects** by reasoning about **causal connections**.
  - AI needs to **learn to do the same**.

## Video ID: Jy09USz_79E
### EBL in Raven’s Progressive Matrices
- **How can AI apply EBL?**
  - AI can **explain transformations** in patterns.
  - Uses **prior knowledge of transformations** (e.g., rotation, reflection).
  - Transfers that knowledge to solve **new problems**.

## Video ID: ISxVJKvvJ18
### Summary: Explanation-Based Learning
- **Key Takeaways**:
  - **Concept Space**: Mapping relationships between concepts.
  - **Prior Knowledge**: AI retrieves existing concepts to solve problems.
  - **Abstraction**: Extracting general rules.
  - **Transfer Learning**: Applying knowledge to new situations.
- **Next Topic**: **Analogical Reasoning**.

## Video ID: FWmC6qILKV8
### The Role of Explanation in AI Trust
- **Why Explanations Matter**:
  - AI **must justify its decisions**.
  - Example: **Medical diagnosis systems must explain reasoning**.
- **Challenges in Explanation**:
  - **Humans are not always good at explaining** (e.g., unconscious skills).
  - AI’s explanation **may differ from the real reasoning process**.
- **Final Thought**:
  - AI that **explains its reasoning** will be **more trusted and widely accepted**.

