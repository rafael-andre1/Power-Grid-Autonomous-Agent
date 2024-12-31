# Power Grid Multi-Agent System 


This project, developed for **Introduction to Intelligent and Autonomous Systems**, models the popular board game **Power Grid** using a **Multi-Agent System (MAS)** framework. The aim was to simulate the complex interactions between players and the game environment while adhering to the core rules and maintaining strategic depth.

The MAS framework includes distinct agents for managing game flow and simulating player behaviors, along with a robust environment representation.


The work was carried out by:

 - **Eduardo Passos**
 - **Pedro Fernandes**
 - **Rafael Pacheco**
 
For a general development and results review: **`presentation.pptx`**

\
**Thank you for exploring this project! You can find the original repository [here](https://github.com/Jumpitas/Power-Grid.git)! 💡**

---

## Game Overview

In Power Grid, players compete to build up electrical networks from scratch and be the player to power the most cities at the end of the game.

Each player represents a company which owns power plants and tries to supply electricity to cities.

### Objective:
To develop a functional MAS that supports:
- Game flow management.
- Player agent decision-making.
- Environmental state maintenance.


The objective of Power Grid is to supply the most cities with power when someone's network gains a predetermined size.

In this project we planned and created the interactions between the board, and the players, in the different phases of the game.

Some rules were simplified, due to the non-impact they would have on the interactions among agents, and the difficulty of programming them efficiently.


---

## System Components

### **Game Manager Agent**
- Manages the sequence of game phases and sub-phases.
- Conducts auctions and oversees resource/environment updates.
- Operates as a **Simple Reflex Agent**, purely reactive and non-adaptive.

### **Player Agent**
Simulates the behavior of a human player:
  - Makes decisions based on game state and inventory.
  - Adapts strategies to the current game phase and available resources.
  - Implemented as a **Model-Based Reflex Agent**, allowing variability within predefined decision rules.

### **Environment**
Represents the board, including:
  - US map graph (nodes and edges).
  - Player inventories (resources, cities, funds).
  - Power plant market and associated resources.
  - Acts as a passive entity, providing a static representation of game information.

---

## Experimentation

### Robustness Testing
- Ensured rule compliance and seamless agent interactions under various scenarios.
- Assessed strategic adaptability and dynamic behavior.

### Customization
- Configurable player count (2–6) via `main.py`.
- Adjustable initial setup, including resources, power plants, and prices.
- Rule-compliant modifications to test diverse game conditions.

### Non-Linear Behavior
Incorporated probabilistic elements for realistic decision-making:
  - Players avoid spending all funds, prioritizing city expansion.
  - Randomized power plant purchases simulate diverse strategies.

---

## Key Insights

- The MAS effectively simulates Power Grid’s strategic complexity.
- Robust agent interactions ensure adherence to rules and gameplay integrity.
- Randomized decisions enhance realism and create varied gameplay scenarios.
- Elevated customizability and functionalities.
