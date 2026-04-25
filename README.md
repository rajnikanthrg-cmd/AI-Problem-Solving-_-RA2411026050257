# 🤖 AI Problem Solving Assignment
**SRM Institute of Science and Technology**  
**Register Number:** RA2411026050257  

![Language](https://img.shields.io/badge/Language-HTML%20%7C%20JS%20%7C%20CSS-yellow)
![Problems](https://img.shields.io/badge/Problems-3-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Submitted-success)

---

## 📋 Problems Overview

| Problem # | Title | Algorithm | Difficulty |
|-----------|-------|-----------|------------|
| Problem 5 | Map Coloring Solver | CSP + Backtracking + MRV | 🟢 Easy |
| Problem 11 | GPS City Route Finder | A* + Dijkstra | 🟡 Medium |
| Problem 1 | Tic-Tac-Toe AI | Minimax + Alpha-Beta Pruning | 🔴 Hard |

---

## 🟢 Problem 5 — Map Coloring (CSP)
**What it does:**  
An interactive visualizer that colors a generic map ensuring no two adjacent regions share the same color. It dynamically demonstrates how the algorithm assigns colors and backtracks when a conflict occurs.

**Algorithm:** Backtracking CSP with Forward Checking and MRV heuristic  
**Features:** interactive graph builder, animated solving, stats panel  
**Sample:** A→Red, B→Green, C→Blue, D→Red  

![Problem 5 Map Coloring](./Problem5_MapColoring/preview.png)


---

## 🟡 Problem 11 — GPS Route Finder (A*)
**What it does:**  
A map-based routing simulation that calculates the shortest path between a starting city and a destination. It allows users to place nodes (cities) and define edges (roads) with associated distance weights.

**Algorithm:** A* Search with Euclidean heuristic vs Dijkstra  
**Features:** click-to-build graph, animated pathfinding, comparison table  
**Sample:** A→B→D→F, Cost=6, A* explored 3 nodes vs Dijkstra 6 nodes  

![Problem 11 GPS Route Finder](./Problem11_GPSRouteFinder/preview.png)


---

## 🔴 Problem 1 — Tic-Tac-Toe AI (Minimax)
**What it does:**  
An unbeatable Tic-Tac-Toe agent that plays flawlessly against human opponents. It includes an interactive analytics display to evaluate how the AI anticipates future moves.

**Algorithm:** Minimax + Alpha-Beta Pruning, Human vs AI and Human vs Human  
**Features:** two game modes, algorithm toggle, comparison panel, move log  
**Performance:** AI never loses on hard mode  

![Problem 1 Tic-Tac-Toe AI](./Problem1_TicTacToe/preview.png)


---

## 📁 Repository Structure

```text
AI-Problem-Solving-_-RA2411026050257/
├── Problem5_MapColoring/
│   └── index.html
├── Problem11_GPSRouteFinder/
│   └── index.html
├── Problem1_TicTacToe/
│   └── index.html
└── README.md
```

---

## 🚀 How to Run

1. **Clone repo:**
   ```bash
   git clone https://github.com/rajnikanthrg-cmd/AI-Problem-Solving-_-RA2411026050257.git
   ```
2. **Open** any problem's `index.html` directly in your browser.
3. **No installation needed!** The applications are fully self-contained.

---

## 🧠 Algorithms Covered

- **CSP**
- **Backtracking**
- **Forward Checking**
- **MRV (Minimum Remaining Values)**
- **A* Search**
- **Dijkstra's Algorithm**
- **Euclidean Heuristic**
- **Minimax Algorithm**
- **Alpha-Beta Pruning**

---

## 📝 Assignment Details

- **Course:** Artificial Intelligence
- **Institution:** SRM Institute of Science and Technology
- **Deadline:** 25th April 2026
- **Submission:** GitHub Repository

---

## 📜 License

This project is licensed under the **MIT** License.
