# Lecture 14: Understanding in AI

###### Video ID: 2FyBCtHrxYs
### Introduction to Understanding
- **Understanding**: The process of making sense of stories and the world.
- **Key concepts**:
  - **Frames**: A knowledge representation system.
  - **Thematic Role Systems**: A structured type of frame representation.
  - **Grammar & Constraints**: Help guide the interpretation of ambiguous concepts.
- **Upcoming topic**: **Common sense reasoning**.
![[Screenshot 2025-03-05 at 11.25.23 AM.png]]
###### Video ID: 1fke7NxJSiE
### Story Understanding and Disambiguation

![[Screenshot 2025-03-05 at 11.25.54 AM.png]]

- **Two stories with the word "kill"**:
  - **Earthquake story**: "Kill" means *causing death*.
  - **President's story**: "Kill" means *rejecting proposals*.
- **Humans structure information through stories**:
  - Background knowledge helps in understanding.
  - AI programs require structured approaches to **disambiguate meanings**.
- **Goal**: Teach an AI system to differentiate between meanings based on context.

![[Screenshot 2025-03-05 at 11.27.32 AM.png]]


###### Video ID: TNpppu_KAqU
### Sentence Analysis: "Ashok made pancakes for David with a griddle."
- **Types of analysis**:
  - **Lexical analysis**: Identifies parts of speech.
  - **Syntactic analysis**: Examines sentence structure.
  - **Semantic analysis**: Defines relationships within the sentence.
- **Thematic Roles**:
  - **Agent**: Ashok (the doer).
  - **Action**: Made (the verb).
  - **Object**: Pancakes.
  - **Beneficiary**: David.
  - **Instrument**: Griddle.
- **Inference in Understanding**:
  - AI should infer that David probably ate the pancakes.
  - Inference-based understanding mirrors human cognition.
![[Screenshot 2025-03-05 at 11.30.07 AM.png]]

###### Video ID: hASvnAHHdcs
### Thematic Role Systems in AI
- **Definition**: A [[7 Frames]] -based system where each action has associated expectations.
- **Example**: The verb "throw" expects:
  - **Agent**: Someone throwing.
  - **Object**: Something being thrown.
  - **Target/Destination**: The recipient or direction of the throw.
- **Role of Thematic Frames**:
  - Helps AI **predict missing information**.
  - Generates expectations even when details are missing.

###### Video ID: eR2feVVPmdU
### Story Representation: "David went to the meeting with Ashok by car."
- **Breaking it down**:
  - **Verb**: Went (past tense of "go").
  - **Agent**: David.
  - **Co-agent**: Ashok.
  - **Destination**: The meeting.
  - **Conveyance**: Car.
- **Challenge**: How does AI determine these roles?
![[Screenshot 2025-03-05 at 11.33.58 AM.png]]

![[Screenshot 2025-03-05 at 11.35.50 AM.png]]
###### Video ID: WtG4eI4uers
### Using Grammar & Prepositions for Meaning
- **Example**: "By" can mean:
  - **Agent** → "Written by Ashok."
  - **Conveyance** → "Went by train."
  - **Location** → "Stood by the statue."
  - ![[Screenshot 2025-03-05 at 11.36.20 AM.png]]
- **AI Needs Additional Knowledge**:
  - Prepositions impose constraints but do not fully determine meaning.
  - **Ontology of the World**: Helps determine if a noun is an agent, object, or location.
![[Screenshot 2025-03-05 at 11.36.49 AM.png]]
###### Video ID: vWPReLEy0AA
### The Role of Ontologies in AI Understanding
- **Ontology**: A structured categorization of the world.
- **Example**:
  - Ashok → Person → Agent.
  - Train → Object → Conveyance.
  - Statue → Object → Location.
- **Bottom-Up vs. Top-Down Processing**:
  - **Bottom-Up**: Starts with words and builds meaning.
  - **Top-Down**: Uses knowledge to guide interpretation.
- **Key Insight**: **Humans rely on background knowledge to interpret meaning**.

###### Video ID: s6e1Aycar8A
### Word Ambiguity and Humor
- **Puns rely on multiple interpretations**:
  - *"I was wondering why the ball was getting bigger, then it hit me."*
    - **Hit** = *occur to* vs. *physically strike*.
  - *"Kleptomaniacs take things literally."*
    - **Take** = *interpret* vs. *steal*.
- **AI Challenge**: Resolving when **one correct meaning** is necessary vs. **humor** where multiple meanings coexist.

###### Video ID: RTWFkMaxEK0
### Ambiguity in Common Words: "Take"
- **Example meanings** of *take*:
  - **To steal**: "I took the candy from the baby."
  - **To medicate**: "Ashok took aspirin."
  - **To measure**: "The doctor took my blood pressure."
  - **To assume control**: "He took over the company."
- **How AI Disambiguates**:
  - Uses **frame-based representation** of each meaning.
  - Checks for **thematic roles** (e.g., "from" suggests theft, "over" suggests control).
![[Screenshot 2025-03-05 at 11.43.32 AM.png]]

We can look at the sentence and remove choices since they do not work. Looking at candy we know its not medicine, its not something you cheat or swindle, your not transporting, we can eliminate more till we see that steal is the most appropriate


###### Video ID: iqeG0k2sPyo
### AI Disambiguation Exercise
- **Example sentences and correct meanings**:
  1. *"I took 3 from 5."* → **To subtract.**
  2. *"I took my briefcase to work."* → **To carry.**
  3. *"I took $5 million at the casino."* → **To cheat/swindle.**
- **AI requires background knowledge**:
  - Numbers are not objects or destinations → "Take" must mean subtraction.
  - "From" suggests a source → "Take" must mean theft.
  - Context impacts interpretation.

###### Video ID: nQjfI8Wc-4o
### Disambiguating "Kill" in Stories
- **Meanings of "Kill"**:
  - *To cause death* → "The earthquake killed 25 people."
  - *To put an end to something* → "The president killed 25 proposals."
- **How AI Differentiates**:
  - **Victim vs. Object**: People vs. Proposals.
  - **Agent's role**: Natural disaster vs. Government official.
  - **Background Knowledge**: Helps infer correct meaning.

###### Video ID: wijBXftv-0c
### Applying Understanding to Raven's Progressive Matrices
- **Cognitive AI Challenge**:
  - Identifying **patterns and transformations**.
  - Frames help define **expected changes**.
  - **Degree of fit** to an expected transformation determines accuracy.

###### Video ID: ewKG0zwKzXo
### Summary: Understanding in AI
- **Key takeaways**:
  - **Frames & Thematic Role Systems**: Capture verbs and expected roles.
  - **Ambiguity Resolution**: Uses background knowledge & constraints.
  - **Grammar & Structure**: Helps guide interpretation.
- **Next topic**:
  - **Multiple words/sentences with the same meaning**.
  - **How AI recognizes and processes semantic equivalence**.
