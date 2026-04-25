<div align="center">

# 🗺️ Map Coloring Solver

[![Algorithm](https://img.shields.io/badge/Algorithm-CSP%20Backtracking-blueviolet.svg?style=for-the-badge)](https://en.wikipedia.org/wiki/Constraint_satisfaction_problem)
[![Language](https://img.shields.io/badge/Language-HTML%2FCSS%2FJS-blue.svg?style=for-the-badge)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Status](https://img.shields.io/badge/Status-Live%20Demo-success.svg?style=for-the-badge)](https://bunny276-luffy.github.io/Map-Colouring/)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

*An interactive, high-performance visualization of the Constraint Satisfaction Problem (CSP).*

[![Live Demo](https://img.shields.io/badge/▶_LIVE_DEMO-Click_Here-ff3366?style=for-the-badge&logo=github)](https://bunny276-luffy.github.io/Map-Colouring/)

</div>

---

## 🧠 About the Project

The **Map Coloring Problem** is a fascinating mathematical puzzle and a classic **Constraint Satisfaction Problem (CSP)**. The core objective is beautifully simple: assign a specific color to each region of a map so that no two bordering regions share the same color. 

While it looks like a simple coloring game, this problem is foundational to artificial intelligence and computer science. It directly models real-world logistical nightmares such as **frequency assignment for cellular networks**, **register allocation in compilers**, and **complex time-table scheduling**.

*This project was developed as **Problem 5 — CSP** for the AI Problem Solving Assignment at SRM Institute of Science and Technology.*

---

## ⚙️ The Algorithm Explained

This solver doesn't just guess colors; it systematically hunts for the solution using three powerful AI concepts:

### 1. Constraint Satisfaction Problem (CSP)
A CSP consists of **Variables** (the regions), **Domains** (the available colors), and **Constraints** (adjacent regions cannot have the same color). The goal is to find a complete assignment that violates zero constraints.

### 2. Backtracking with Forward Checking
Instead of blindly searching, the algorithm acts like a smart detective:
* **Backtracking**: It colors one node at a time. If it paints itself into a corner (a node has no valid colors left), it immediately "backtracks" to the previous node and tries a different color path.
* **Forward Checking**: Every time a node is colored, the algorithm looks ahead and removes that color from the "available colors" list of all its unassigned neighbors. If a neighbor's list becomes empty, it instantly knows the current path is doomed, saving thousands of wasted calculations!

### 3. MRV Heuristic (Minimum Remaining Values)
Also known as the "fail-first" principle. The algorithm dynamically chooses to color the hardest, most constrained region next—specifically, the one with the fewest legal colors left.

#### 💡 The Solve Process (ASCII Visualization)
```text
[A] --- [B]     Colors: [Red, Green, Blue]
 | \   / |      
 |  \ /  |      Step 1: Pick A (MRV) -> Assign Red
 |  / \  |      Step 2: Forward Check -> Remove Red from B,C
[C] --- [D]     Step 3: Pick B -> Assign Green
                Step 4: Pick C -> Assign Blue
                Step 5: Pick D -> Assign Red (Valid!)
```

---

## ✨ Stellar Features

* 🎨 **Interactive Builder**: Add custom regions and define adjacency rules on the fly.
* ⚡ **Real-Time Visualization**: Watch the algorithm "think" as it traverses and colors the graph.
* 📊 **Live Telemetry**: Real-time stats panel tracking Nodes Explored, Backtracks, Calculation Time, and Colors Used.
* 🌈 **Cyberpunk Aesthetic**: Gorgeous "neural circuit board" UI featuring neon glows, particle ripples, and dynamic layouts.
* 🔄 **Step-by-Step Animation**: See the backtracking algorithm backtrack in real-time.
* 📱 **Zero Dependencies**: 100% Vanilla JavaScript, HTML5 Canvas, and pure CSS.

---

## 🚀 How to Run

Because this is a completely dependency-free, self-contained application, running it is incredibly easy:

### Option 1: Live Demo
Simply click the link below to run it directly in your browser:
**👉 [Play the Live Demo Here](https://bunny276-luffy.github.io/Map-Colouring/)**

### Option 2: Local Execution
1. Clone this repository or download the `index.html` file.
2. Double-click `index.html` to open it in Chrome, Firefox, Safari, or Edge.
3. *No installations, no servers, no NPM required!*

---

## 🧪 Sample Input & Output

Based directly on the assignment criteria.

**Input Configuration:**
```text
Regions: A, B, C, D
Adjacency: 
  A -> B, C
  B -> A, C, D
  C -> A, B, D
  D -> B, C
Colors: 3 (Red, Green, Blue)
```

**Solved Output:**
```text
A -> Red
B -> Green
C -> Blue
D -> Red
```

---

## 📁 Project Structure

```text
Map-Colouring/
├── index.html        # Main application (self-contained logic & styling)
└── README.md         # You are here
```

---

## 👨‍💻 Author

**Made with ❤️ by Yashasvi Beesam**

* B.Tech Artificial Intelligence & Machine Learning
* SRM Institute of Science and Technology (2024–2028)
* [GitHub Profile](https://github.com/Bunny276-luffy)
* *Part of AI Problem Solving Assignment — SRM University*

---

## 📜 License

This project is licensed under the MIT License.
