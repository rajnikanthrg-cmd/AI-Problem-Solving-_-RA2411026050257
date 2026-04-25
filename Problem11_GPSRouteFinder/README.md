# 🗺️ GPS City Route Finder — A* Algorithm

![Algorithm](https://img.shields.io/badge/Algorithm-A*-blue.svg)
![Language](https://img.shields.io/badge/Language-HTML%2FCSS%2FJS-yellow.svg)
![Status](https://img.shields.io/badge/Status-Live-brightgreen.svg)
![License](https://img.shields.io/badge/License-MIT-orange.svg)

**Live Demo:** [https://bunny276-luffy.github.io/GPS-Route-Finder/](https://bunny276-luffy.github.io/GPS-Route-Finder/)

> An interactive web-based visualizer solving spatial pathfinding using the A* Search Algorithm.

---

## 📖 About
This project is an interactive Graph/GPS Pathfinding visualizer built entirely in Vanilla JS within a single HTML file. It allows users to place city nodes, connect them with weighted edges, and watch the A* Search Algorithm dynamically find the optimal route. 

**Real-world Relevance:** Algorithms like A* and Dijkstra form the backbone of modern navigation systems, such as Google Maps and GPS routing, solving the shortest-path problem efficiently across massive network grids.

**Assignment Context:** This project was developed as part of the AI Problem Solving Assignment — Problem 11 for the B.Tech Artificial Intelligence & Machine Learning program at SRM Institute of Science and Technology.

---

## 🧠 Algorithm Explanation

### A* Search
The A* (A-Star) algorithm is an informed search algorithm heavily used in pathfinding and graph traversal. It evaluates nodes by combining the exact path cost incurred so far with the estimated cost to reach the goal.

The core formula is:
**`f(n) = g(n) + h(n)`**
- **`g(n)`**: The exact path cost from the start node to the current node `n`.
- **`h(n)`**: The heuristic (estimated) cost from the current node `n` to the goal node.
- **`f(n)`**: The total estimated cost of the path passing through node `n`.

### The Heuristic
A* requires an admissible heuristic (one that never overestimates the true cost) to guarantee finding the optimal path. Since our nodes represent physical coordinate cities on a canvas, we use the **Euclidean Distance** formula:
```text
h(n) = √((x2 - x1)² + (y2 - y1)²)
```
*(Scaled proportionally to edge weights to guarantee admissibility).*

### A* vs Dijkstra: Why A* is Better
Dijkstra's Algorithm is an uninformed search that explores blindly in all directions. A*, guided by its heuristic, searches directionally toward the target goal.
In our project's default spatial graph:
- **A* explored:** 3 nodes
- **Dijkstra explored:** 6 nodes

A* calculates the exact same optimal path but completely avoids exploring branches that head in the wrong direction!

### A* Pseudocode
```text
1. Initialize openSet with startNode
2. While openSet is not empty:
3.    current = node in openSet with lowest f(n)
4.    if current is goal: return reconstructed path
5.    remove current from openSet, add to closedSet
6.    for each neighbor of current:
7.        if neighbor in closedSet: continue
8.        tentative_g = g(current) + edge_weight(current, neighbor)
9.        if tentative_g < g(neighbor):
10.           update cameFrom[neighbor] = current
11.           update g(neighbor) and f(neighbor)
12.           add neighbor to openSet
```

---

## ✨ Features
- 🖱️ **Click-to-place**: Interactive canvas to dynamically place city nodes.
- 🔗 **Weighted Edges**: Click two nodes sequentially to add an edge and assign a distance/weight.
- ⚡ **Animated Pathfinding**: Watch the algorithm explore with color-coded states (yellow for frontier, gray for visited).
- 📊 **Real-time Comparison**: View an instant performance table comparing A* vs Dijkstra.
- 📝 **Exploration Log**: Scrollable step-by-step history showing exact `f`, `g`, and `h` calculations.
- 🎯 **Preloaded Graph**: Ready-to-solve spatial map loaded by default.
- 🌙 **Dark UI Aesthetics**: Beautiful neon glow paths against a deep space dark theme.

---

## 🛠️ Sample Input / Output
**Graph Setup:**
- Edges: `A→B(1)`, `A→C(4)`, `B→D(2)`, `B→E(5)`, `C→D(1)`, `D→F(3)`, `E→F(1)`

**Execution:**
- **Start City:** A
- **Goal City:** F

**Output:**
- **Optimal Path:** `A → B → D → F`
- **Total Path Cost:** `6`
- **Performance:** A* nodes explored: **3**, Dijkstra nodes explored: **6**

---

## 🚀 How to Run
There are absolutely no dependencies or installations required!

1. **Option 1 (Local):** Clone the repository to your machine and simply double-click `index.html` to open it in any modern web browser (Chrome, Safari, Edge, Firefox).
2. **Option 2 (Live):** Visit the [Live GitHub Pages Demo](https://bunny276-luffy.github.io/GPS-Route-Finder/).

---

## 📁 Project Structure
```text
GPS-Route-Finder/
├── index.html   # Full application (HTML, CSS, JS)
└── README.md    # Documentation
```

---

## 👨‍💻 Author
**Yashasvi Beesam**  
🎓 B.Tech Artificial Intelligence & Machine Learning (2024–2028)  
🏛️ SRM Institute of Science and Technology  

## 📄 License
This project is licensed under the [MIT License](LICENSE).
