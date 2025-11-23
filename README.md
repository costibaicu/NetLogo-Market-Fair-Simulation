# 🎡 Agent-Based Simulation: Market Fair Dynamics

This project is an agent-based model (ABM) developed in **NetLogo** for the **Fundamentals of Economic Cybernetics** course at **CSIE - ASE Bucharest**.

The simulation models the behavior of visitors at a market fair ("târg"), focusing on goal fulfillment, state transitions, and environmental adaptability.

## 📝 Simulation Logic

The model simulates a closed system representing a market with two primary agents: **Visitors** (mobile agents) and **Stalls** (stationary agents).

### 🔍 Core Rules & Cybernetic Principles
1.  **Goal-Oriented Behavior:**
    * **Entry State (Red):** Visitors enter the fair represented as **red** agents. They are in a "browsing" or "unsatisfied" state.
    * **Interaction:** Agents move randomly to find and "visit" stalls.
    * **Threshold (Feedback Loop):** A specific counter tracks the number of unique stalls visited. The threshold is set to **minimum 2 stalls**.
    * **Exit State (Green):** Upon visiting the 2nd stall, the agent changes color to **green** (representing "satisfied") and exits the system (leaves the fair).

2.  **Environmental Adaptation (Time of Day):**
    * The simulation features a dynamic **Day/Night cycle**.
    * **Daytime:** Agents move at standard/faster speed, representing high energy and visibility.
    * **Nighttime:** Agents significantly reduce their movement speed, simulating fatigue or low visibility.

## 📂 Project Structure
* `Proiect BCE.nlogo`: The main source code containing the interface, turtle/patch logic, and the `go` procedure.
* `Proiect BCE world.csv`: Configuration data for the initial world state.
* `Proiect BCE code.html`: HTML export of the codebase.

## 🚀 How to Run
1.  Download and install **NetLogo** (Version 6.x).
2.  Open `Proiect BCE.nlogo`.
3.  **Interface Controls:**
    * Click **Setup** to initialize the stalls and the clock.
    * Click **Go** to start the visitor flow.
    * Use the **Time** sliders (if available) to manually adjust the hour or observe the automatic cycle.
4.  **Observation:** Watch as red agents turn green after their interactions and observe the speed change as the simulation hour passes into the "night" zone.

## 📊 Cybernetic Concepts Applied
* **Adaptive Systems:** Agents alter their state (color) based on accumulated history (memory of visits).
* **System Constraints:** The environment (Time) acts as a regulator on the system's throughput (Speed).
* **Negative Feedback:** The "leaving" mechanism prevents overcrowding by removing satisfied agents.

---
*Student Project | Faculty of Cybernetics, Statistics, and Economic Informatics (CSIE)*
