# 🎮 Tic-Tac-Toe AI — Minimax vs Alpha-Beta Pruning

![Algorithm](https://img.shields.io/badge/Algorithm-Minimax%20%7C%20Alpha--Beta-blue)
![Language](https://img.shields.io/badge/Language-Vanilla%20JS-yellow)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![License](https://img.shields.io/badge/License-MIT-green)

**Author:** Yashasvi Beesam, B.Tech AI & ML, SRM University 2024-2028  
**Live Demo:** [https://bunny276-luffy.github.io/TIC-TAC-TOE/](https://bunny276-luffy.github.io/TIC-TAC-TOE/)

## About
This project is an interactive, self-contained Tic-Tac-Toe game built from scratch using HTML, CSS, and Vanilla JavaScript. It serves as a visual and analytical demonstration of game theory algorithms, specifically comparing the performance of the **Minimax** algorithm against its optimized variant, **Alpha-Beta Pruning**.

## Algorithm Explanation

### Minimax
The Minimax algorithm is a decision-making tool used in artificial intelligence, game theory, and decision theory. It evaluates the entire game tree to find the optimal move, assuming the opponent is also playing optimally.
- **Game Tree:** The algorithm explores all possible future moves down to the terminal states (win, loss, or draw).
- **Process:** The "Maximizing" player tries to get the highest score, while the "Minimizing" player tries to get the lowest score. The algorithm works recursively from the leaves up to the root.

### Alpha-Beta Pruning
Alpha-Beta Pruning is an optimization technique for the Minimax algorithm. It reduces the number of nodes evaluated by the minimax algorithm in its search tree.
- **How it works:** It maintains two values, Alpha and Beta, which represent the minimum score that the maximizing player is assured of and the maximum score that the minimizing player is assured of, respectively.
- **Pruning:** If at any point the algorithm finds that a branch cannot possibly influence the final decision (because a better option was already found), it "prunes" or completely skips evaluating that branch.

### Comparison
| Algorithm | Completeness | Efficiency | When to use |
|-----------|--------------|------------|-------------|
| Minimax | Explores 100% of nodes | Slow | Small search spaces |
| Alpha-Beta | Explores ~10-50% of nodes | Fast | Deeper search trees |

Alpha-Beta guarantees the exact same optimal decision as Minimax, but achieves it significantly faster by avoiding redundant computations.

## Features
- 🤖 Unbeatable AI using Optimal Game Theory
- ⚖️ Live toggle between Minimax and Alpha-Beta algorithms
- 📊 "Both" mode for real-time node exploration comparison
- 📈 Visual CSS bar charts showing efficiency differences
- 📝 Detailed Step Log for each move and AI thought process
- 🎨 Premium Dark Theme with neon glow effects
- 🏆 Score tracking across sessions

## Sample Game Output
*Move 3: AI played position 4 using Alpha-Beta (explored 19 nodes in 0.2ms)*
*Alpha-Beta pruned 87% of nodes compared to Minimax.*

## How to Run
1. Download the `index.html` file.
2. Double-click the file to open it in any modern web browser.
3. No build tools, servers, or external dependencies required!

## Project Structure
- Single `index.html` file containing:
  - **HTML:** Semantic layout and panels.
  - **CSS:** Inline styles with CSS variables and flex/grid layouts.
  - **JS:** Core game logic, algorithmic implementations, and UI state management.

## License
MIT License
