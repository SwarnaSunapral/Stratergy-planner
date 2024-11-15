```markdown
# Sliding Blocks Puzzle 🧩

Welcome to the **Sliding Blocks Puzzle**! This repository implements a `3x3` sliding block puzzle using **A* search algorithm** with various heuristics. Solve the puzzle efficiently with the sum of Manhattan distances as the primary heuristic. 🚀

---

## 📝 Description  

The sliding blocks puzzle consists of a `3x3` grid of numbered tiles (0 to 8). The goal is to rearrange the tiles to match the **goal configuration**, starting from a random initial state. The blank tile (denoted as `0`) can swap places with adjacent tiles to navigate the board.

### Example:
**Initial State**  
```
6 0 5  
1 3 2  
7 8 4  
```

**Goal State**  
```
1 2 3  
4 5 6  
7 8 0  
```

---

## 🔥 Features

- Implements the **A* search algorithm**.
- Supports multiple heuristics:
  - **Manhattan Distance**
  - **Misplaced Tiles**
  - **Zero Manhattan Distance**
- Randomly generates initial states.
- Tracks the number of steps and cells explored.
- Validates whether a path exists to the goal state.

---

## 🚀 How to Run

### Prerequisites
- Python 3.x  
- Install required dependencies:
  ```bash
  pip install -r requirements.txt
  ```

### Running the Puzzle Solver
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/sliding-blocks.git
   cd sliding-blocks
   ```

2. Execute the script:
   ```bash
   python sliding_blocks.py
   ```

---

## 🧠 Heuristics Explained

1. **Manhattan Distance**:  
   Calculates the sum of vertical and horizontal distances of tiles from their target positions.

2. **Misplaced Tiles**:  
   Counts the number of tiles not in their goal positions.

3. **Zero Manhattan Distance**:  
   Computes the Manhattan distance specifically for the blank tile (`0`).

---

## 📊 Example Output

```
SOURCE:
(6, 0, 5)
(1, 3, 2)
(7, 8, 4)

There is a path from (6, 0, 5) to (1, 2, 3)
PATH:
(6, 0, 5)
(1, 3, 2) -->
(7, 8, 4)

...

Number of cells explored = 2127
```

---

## 🔎 Observations

1. Not every initial state has a path to the goal.
2. Board positions are divided into two equivalence classes based on reachability:
   - Positions that can reach the goal.
   - Positions that cannot unless the initial state is modified.

---

## 🛠️ Project Structure

```
sliding-blocks/
├── sliding_blocks.py     # Main script
├── requirements.txt      # Required Python packages
├── README.md             # Project description
└── LICENSE               # License information
```

---

## 🤝 Contributing

We welcome contributions! If you find a bug or have an idea to improve this project:  
1. Fork the repo.  
2. Create your feature branch (`git checkout -b feature/AmazingFeature`).  
3. Commit your changes (`git commit -m 'Add AmazingFeature'`).  
4. Push to the branch (`git push origin feature/AmazingFeature`).  
5. Open a Pull Request.

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 🌟 Acknowledgments

This project is inspired by classic search algorithms and designed to showcase the capabilities of A* search with heuristic-based optimization.

---

## 🚀 Author

Developed by **Sunapral Swarnalatha Bai** ✨
