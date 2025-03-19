
# Lecture 13: Planning in AI

Video ID: yE0lK8CItlE
### Introduction to Planning
- **Definition**: An intelligent agent maps perceptual histories into actions.
- **Planning**: A method for action selection using logical syntax.
- **Key concepts**:
  - **Goals and States**: Specifications for what the agent wants to achieve.
  - **Operators**: Define how an agent moves between states.
  - **Conflicts between multiple goals**: Addressed by **partial-order planning**.
  - **Hierarchical Task Networks (HTNs)**: Used for complex hierarchical plans.

Video ID: if0YnRb9iEU
### Blocks World Problem
- **Scenario**: A robot moves blocks from an initial state to a goal state.
- **Constraints**:
  - Robot has one arm → moves one block at a time.
  - Can only move a block if no other block is on top.
- **Comparison of approaches**:
  - **Weak AI (Means-Ends Analysis)**: Previously considered.
  - **Systematic, knowledge-based methods**: Now used for structured goal selection.
- **Question**: How does an agent select the most relevant goal?

Video ID: Xa3Yq6fw4Tk
### Goal Conflict Example: Painting a Room
- **Scenario**: Robot must paint both the ceiling and the ladder.
- **Conflict**: If the robot paints the ladder first, it cannot climb it to paint the ceiling.
- **Solution**: **Order of actions matters**:
  - **Correct order**: Paint the ceiling first, then the ladder.
  - **AI Reasoning**: Using **propositional logic** to represent goals.


Video ID: OxRwB46NXuM
### Propositional Logic Representation
- **Exercise**: Represent "painting the ladder" using propositional logic.
- **Combining goals**: Represent both "Painted(Ceiling)" and "Painted(Ladder)" as a conjunction.

Video ID: ZAp8yyEiVBA
### Specifying the Initial State
- **Example**:
  - **Initial state**: Robot is on the floor, ladder and ceiling are dry.
  - **Goal state**: Ladder and ceiling are painted.
- **Fully specifying a goal**: Requires both **initial and goal states**.

![[Screenshot 2025-03-04 at 2.30.23 PM.png]]


Video ID: 2PyyQt1Vcmg
### Defining Operators in Planning
- **Example**: Operator **climb-ladder**
  - **Precondition**: Robot is on the floor, ladder is dry.
  - **Postcondition**: Robot is on the ladder.
- **Key Rules**:
  - **Preconditions must be positive literals**.
  - **Postconditions may include negative literals**.
- ![[Screenshot 2025-03-04 at 2.34.28 PM.png]]

![[Screenshot 2025-03-04 at 2.40.18 PM.png]]

in example paint-ceiling we need to negate things that were true in the world before, ex `paint-ladder` we need to negate truths previously. We need to state the ladder is not dry now.  


Video ID: v6zTfqhtEhc
### Exercises: Defining Operators
- **Examples**:
  - **descend-ladder**: Preconditions → robot on ladder, ladder dry. Postcondition → robot on floor.
  - **paint-ceiling**: Preconditions → robot on ladder. Postconditions → ceiling painted, ladder not dry.
  - **paint-ladder**: Preconditions → robot on floor. Postconditions → ladder painted, ladder not dry.
  
Video ID: 3K8KUD_D6ds
### Planning and Navigation
- **Example**: Navigating an urban area
- **Types of Knowledge**:
  - **World knowledge**: Intersections, states, operators.
  - **Control knowledge**: How to select operators (heuristics).
- **Means-Ends Analysis**: Uses goals as control knowledge to select operators.

Planning provides systematic methods for selecting diff operators 
![[Screenshot 2025-03-04 at 2.45.30 PM.png]]
![[Screenshot 2025-03-04 at 2.49.32 PM.png]]
Video ID: Xe89wPuPgCc
### Issues with Means-Ends Analysis
- **Problem**: Selecting actions in the wrong order leads to goal conflicts.
- **Example**:
  - **Painting ladder first** → Ladder is wet → Cannot climb.
  - **Painting ceiling first** → No issue.
- **Linear Planners**: Do not handle conflicts well.
We see in the example after doing paint ladder then going into climb ladder the precondition does not match the post condition of paint ladder leads to contradiction

![[Screenshot 2025-03-04 at 2.52.09 PM.png]]


How does planning find out which order to do things
Video ID: Lh8tzE7B6pc
### Introduction to Partial-Order Planning
- **Partial-Order Planning**: Solves conflicts between goals.
- **Example**: Furniture assembly mistake (couch assembly before moving it in the house).
- **Solution**: **Plan steps carefully to avoid conflicts**.


Video ID: cwjbtxddJt8
### Implementing Partial-Order Planning
- **Example**: Painting the ladder and painting the ceiling.
- **Steps**:
  - Identify **goal conditions**.
  - Select **operators that satisfy goal conditions**.
  - **Order operators** to prevent conflicts.

It would break them into sub goals and see what the plan is to achieve that goal
![[Screenshot 2025-03-04 at 3.04.42 PM.png]]

Video ID: nAImor8mgwA
### Conflict Resolution in Partial-Order Planning
- **Detecting conflicts**: Precondition of an operator contradicts another operator's postcondition.
- **Example**: Dry ladder (needed for climbing) becomes wet after painting.
- **Solution**: **Reordering actions or inserting necessary steps (e.g., waiting for ladder to dry).**
![[Screenshot 2025-03-04 at 3.06.34 PM.png]]

![[Screenshot 2025-03-04 at 3.04.42 PM.png]]
### Detecting Conflicts
1.  1st check it pre condition of 1st plan, painted-ladder are "clobbered by" painted-ceiling (doesnt happen this example)
2. Look at 2nd plan, painted-ceiling and see it that has conflict, **It does**![[Screenshot 2025-03-04 at 3.10.45 PM.png]]
	1. We see that there is a contradiction from 2nd plans precondition to the 1st plans post condition

![[Screenshot 2025-03-04 at 3.12.31 PM.png]]

the final plan:
![[Screenshot 2025-03-04 at 3.14.11 PM.png]]
Here the robot needs to find a transition state to lead from plan 1 to plan 2, it finds that `desend-ladder` is best option


Video ID: 7L3tcoFMR7w

Instead of micro operators can we have macro operators to generalize?
![[Screenshot 2025-03-04 at 3.28.53 PM.png]]

### Hierarchical Task Networks (HTN)
- **HTN Planning**:
  - Uses **macro-operators** instead of low-level steps.
  - Makes **complex planning more manageable**.
- **Example**:
  - **Unstack**: Abstract operation for moving blocks.
  - **Stack-Ascending**: Abstract operation for stacking blocks in order.

Video ID: 5wFbZSTumHs
### Planning and Cognitive Agents
- **Why Planning Matters**:
  - **Action selection is central to cognition**.
  - **Humans**: Plan actions (e.g., cooking, traveling, budgeting).
  - **AI**: Needs structured methods to plan multiple goals.
- **Goal Conflicts**:
  - Some goals are complementary.
  - Some goals interfere and require resolution.

