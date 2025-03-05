# Lecture 16: Scripts in AI

## Video ID: FuSqFZBwN_w
### Introduction to Scripts
- **Definition**: Scripts are a structured knowledge representation for understanding discourses, stories, and scenes.
- **Building on previous topics**:
  - **Frames** and **common sense reasoning** contribute to script formation.
  - **Understanding** of causality and expectations helps structure scripts.
- **Key Concepts**:
  - Form and content of scripts.
  - Generating expectations about discourse and stories.
  - The **hierarchical nature** of scripts.

## Video ID: nT-VzlzzWe8
### The Importance of Stories in AI
- **Story-based reasoning**:
  - AI (like Watson and Siri) primarily understand **single sentences**.
  - Humans use **stories to provide structure** to information.
- **Example**:
  - *Ali asked, "Do you think we’ll have many customers in the next half hour?"*
  - *Sarah replied, "Go ahead and grab your lunch."*
  - AI must infer Sarah’s reasoning: If no customers are expected, Ali can take a break.

## Video ID: jJOUm3mj-80
### Inferring Meaning and Common Sense
- **Example**:
  - *Ashok wanted to become rich. He got a gun.*
  - Humans infer a **likely causal connection** between obtaining a gun and attempting a robbery.
  - AI must learn to generate such inferences.

## Video ID: wm3pc49x7UE
### Scripts and Common Sense Reasoning
- **Restaurant story**:
  - *Bob went to a restaurant. He waited a long time. His food was burned. He didn’t leave a tip.*
- **AI challenge**: How do we infer the connection?
  - **Scripts help AI connect events logically**.
  - **Pre-learned structures** define relationships between actions and expectations.
  - Roomba- Roomba hears a spill, can imply it needs to clean

## Video ID: bFgtpCAk-UM
### The Power of Scripts in Daily Life
- Humans don’t require **explicit details** in many situations.
- **Example**:
  - At a coffee shop, expectations include:
    - Ordering from a cashier.
    - Receiving a total.
    - Waiting for the drink.
  - If something unusual happens (e.g., the barista slaps you), it violates the expected script.

## Video ID: kW6Zx6hEn-g
### Defining a Script
- **Scripts capture causally coherent events**:
  - **Causal**: One  event leads to another.
  - **Coherent**: The sequence makes logical sense.
- **Example**:
  - Entering a coffee shop leads to ordering, payment, and receiving a drink.

## Video ID: MBOTLKEoxuk
### Structure of a Script
1. **Entry Conditions**: Preconditions required to trigger the script.
   - *Example: Customer is hungry and has money.*
2. **Result**: Expected outcome.
   - *Example: Customer is no longer hungry; restaurant earns money.*
3. **Props**: Objects involved.
   - *Example: Tables, menus, food, cash registers.*
4. **Roles**: Agents performing tasks.
   - *Example: Customer, waiter, cashier, owner.*
5. **Tracks**: Variations of the script.
   - *Example: Fast food vs. fine dining.*
6. **Scenes**: Steps in executing the script.
   - *Example: Entering, ordering, eating, paying, leaving.*

## Video ID: 5V7okCYxdDc
### Example: Restaurant Script Representation
- **Components**:
  - **Props**: Tables, menu, food, money.
  - **Roles**: Customer, waiter, cook, cashier.
  - **Entry Conditions**: Customer is hungry and has money.
  - **Result**: Customer is full, restaurant earns money.
  - **Scenes**:
    - Entering the restaurant.
    - Ordering food.
    - Receiving food.
    - Eating and paying.
![[Screenshot 2025-03-05 at 12.45.34 PM.png]]
![[Screenshot 2025-03-05 at 12.46.02 PM.png]]

## Video ID: zbllXuDBQ0Q
### Instantiating Scripts for AI
- **Example**:
  - A **robot** with a restaurant script can anticipate:
    - What actions it must take.
    - What to expect next.
- **Key Insight**:
  - **Scripts provide a structured guide for AI behavior**.

## Video ID: ZEmIJaGEZoo
### Expectation Violations in Scripts
- **Surprise occurs when expectations aren’t met**.
- **Example**:
  - You sit at a restaurant but don’t receive a menu → **Expectation violation**.
  - You receive the bill before ordering → **Unexpected event**.
- **Theory of Surprise**:
  - **Two types**:
    1. When expected things **do not happen**.
    2. When **unexpected events** occur.
- **Connection to Creativity**:
  - Unexpected events can be **engaging** (e.g., plot twists in movies).
  - Creativity is linked to **novelty, usefulness, and surprise**.


## Video ID: 8j-7Vo93pdc
### Script Tracks: Variations of Common Scripts
- **Examples**:
  - **Restaurant tracks**:
    - Coffeehouse.
    - Fast food.
    - Casual dining.
    - Fine dining.
- **AI and Semantic Hierarchies**:
  - AI can classify a situation into the right **script track**.
  - Example: Recognizing whether a restaurant is fast food or fine dining.
![[Screenshot 2025-03-05 at 12.51.44 PM.png]]


## Video ID: eLE6UenT5Aw
### Learning Scripts in AI
- **Topics that help AI learn scripts**:
  - **Semantic networks**: Represent relationships between concepts.
  - **Frames**: Store structured knowledge.
  - **Incremental learning**: AI refines its understanding over time.
  - **Planning**: Converts plans into reusable scripts.
  - **Common sense reasoning**: Provides logical interpretation of events.

## Video ID: aJPY_z0qt3M
### AI and Script-Based Reasoning
- **AI can use scripts for reasoning**:
  - **Example**:
    - Seeing a hostess at a restaurant → Recognizing a formal dining scenario.
  - **Scripts help AI classify and act efficiently**.

## Video ID: nUB3YEcj0V0
### Using Scripts vs. Generating Scripts
- **AI can either**:
  1. **Use pre-learned scripts**.
  2. **Generate new scripts from experience**.
- **Key Topics**:
  - **Problem reduction**: Breaking down scenes into smaller steps.
  - **Classification**: Identifying the correct script.
  - **Understanding**: Disambiguating between similar events.
![[Screenshot 2025-03-05 at 12.59.13 PM.png]]
![[Screenshot 2025-03-05 at 12.59.24 PM.png]]

## Video ID: o7h0oG3Bzes
### Summary: The Role of Scripts in AI
- **Scripts are essential for understanding and predicting events**.
- **Scripts are hierarchical**:
  - General structure → Specific tracks → Individual instances.
- **Scripts apply to more than just stories**:
  - **Paintings, music, architecture** all convey structured information.
- **Conclusion**:
  - Scripts are a powerful tool in **common sense reasoning**.

## Video ID: hgbPouFelN0
### Scripts and Human Cognition
- **The brain as a prediction machine**:
  - We expect the world to follow **predictable patterns**.
  - When expectations **fail**, we experience **surprise, humor, or frustration**.
- **Mental Models and Culture**:
  - Scripts **vary by culture**.
  - Example: Tipping in the U.S. vs. other countries.
- **Final Thought**:
  - **Do we store scripts permanently, or generate them dynamically?**

