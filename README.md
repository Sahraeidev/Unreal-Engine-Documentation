This detailed document summarizes the key concepts and practical steps taught in the first class, **Unreal Engine Blueprint Fundamentals | Class #1**, focusing on Visual Scripting.

---

# Unreal Engine Blueprint Fundamentals: Class #1 Summary

## 1. Introduction to Visual Scripting & Blueprint

* **Blueprint (BP):** A **visual scripting system** based on connecting nodes. It is a visual way of programming, mostly used for **high-level game design** and implementing in-game logic without writing traditional code.
* **Target Audience:** The class is hyper-focused on teaching programming **foundations** (like variables, loops, and execution flow) to users who lack a traditional programming background.

---

## 2. Blueprint Editor Layout

The Blueprint Editor is the main workspace, designed to house all the visual and functional aspects of an Actor.

| Section | Description | Key Focus in Class |
| :--- | :--- | :--- |
| **Viewport** | Shows the 3D visualization of your Blueprint Actor. | Used to place and visualize components (like the Cube). |
| **Components** | Lists all the visual and functional elements/parts that make up your Blueprint (e.g., Static Mesh, Sphere). | We dragged references of these components into the Event Graph to manipulate them. |
| **Graphs** | Contains the scripting and logic. **Event Graph** is the main workspace. | **Event Graph:** The classroom where visual scripting is done. |
| **Details** | Shows the specific properties and settings for any selected component or node. | Used to set properties like duration, color, and scale. |

---

## 3. Nodes and Execution Flow

* **Node:** An **executable action** (command or function). Different kinds of nodes perform different tasks.
* **Execution Pins (White Triangles):** When nodes are connected by these pins, Unreal executes them sequentially, following the flow from the starting event.

### Core Events

| Event | Function | Class Action |
| :--- | :--- | :--- |
| **Event Begin Play** | Runs **once** at the very start of the level or game experience. | Used as the starting point for all our scripts. |
| **Event Tick** | Runs every single frame (for continuous updates). | Deleted to keep the classroom clean and simple. |

### Essential Nodes for Flow Control

| Node | Purpose | Importance |
| :--- | :--- | :--- |
| **Print String** | Displays text on the screen and/or in the log. | Used for initial demonstration of sequential execution. |
| **Delay** | Pauses the execution flow for a specified duration. | Essential for observing movement/changes that would otherwise happen instantaneously. |
| **Spawn Emitter/Actor** | Creates a new particle system (or other object) in the world. | Used to create an object that we could then manipulate (move). |

---

## 4. Best Practices and Practical Skills

* **Compilation:** You **must Compile** the Blueprint after making any changes (it translates the visual script into machine language). Look for the green checkmark; a red circle indicates an error.
* **Scene Placement:** The Blueprint logic will only run if an instance (copy) of the `BP_Class1_Actor` is **dragged into the level**.
* **Component Reference:** To modify a visual component (like a Static Mesh or Sphere) from the Event Graph, drag it from the **Components** panel into the graph to create a **Reference Node**.
* **Cleanup and Readability:**
    * **Align Nodes:** Select nodes and press **Q** to straighten them for better readability.
    * **Reroute Nodes:** Double-click on a data wire (colored pin) to add a **Reroute Node** to keep the connections clean and easy to follow.
* **Navigation:**
    * **Pan:** **Right-click** and drag to move the graph view.
    * **Zoom:** Hold **Alt + Right-click** and drag to zoom in and out.

---

## 5. Next Steps

The next classes will introduce more powerful concepts to build complex logic:

* **Variables:** For storing data.
* **Control Flow (Logic):** For making decisions (e.g., If/Then statements).
* **Functions:** For making logic reusable.
