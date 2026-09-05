# Practical Assignment 2: Problem Solving through Search

## 📌 Practical Title

**Problem Solving through Search**

This practical demonstrates how Artificial Intelligence techniques can be used to solve problems by searching through possible states and finding suitable paths or solutions.

---

## 🎯 Objectives

* Understand the concept of **problem-solving through search** in Artificial Intelligence.
* Implement different **search algorithms** for solving problems.
* Compare uninformed and informed search techniques.
* Understand the role of **heuristic functions** in informed search.
* Apply **Constraint Satisfaction Problems (CSP)** to solve the N-Queens problem.
* Analyze the solutions produced by different AI search strategies.

---

## 🧠 Algorithms Implemented

The practical covers the following techniques:

### 1. Breadth-First Search (BFS)

BFS explores the search space level by level.

**Characteristics:**

* Complete search strategy.
* Uses a queue.
* Finds the shortest path when all step costs are equal.

---

### 2. Depth-First Search (DFS)

DFS explores one branch of the search tree as deeply as possible before backtracking.

**Characteristics:**

* Uses a stack or recursion.
* Requires less memory than BFS in many cases.
* Does not necessarily find the shortest path.

---

### 3. Greedy Best-First Search

Greedy Best-First Search selects the node that appears closest to the goal according to a heuristic function.

It uses:

```text
f(n) = h(n)
```

where:

* `h(n)` = estimated cost from node `n` to the goal.

---

### 4. A* Search

A* combines the actual cost of reaching a node with the estimated cost to the goal.

It uses:

```text
f(n) = g(n) + h(n)
```

where:

* `g(n)` = cost from the start node to node `n`
* `h(n)` = estimated cost from node `n` to the goal
* `f(n)` = total estimated cost

A* can provide an optimal solution when an appropriate admissible heuristic is used.

---

### 5. Hill Climbing

Hill Climbing is a local search technique that continuously moves toward a better neighbouring state.

**Characteristics:**

* Uses a heuristic evaluation.
* Does not maintain the complete search tree.
* Can get stuck at local maxima, plateaus, or ridges.

---

### 6. N-Queens Problem using CSP

The **N-Queens Problem** is formulated as a Constraint Satisfaction Problem.

The objective is to place `N` queens on an `N × N` chessboard such that no two queens attack each other.

The constraints are:

* No two queens can occupy the same row.
* No two queens can occupy the same column.
* No two queens can occupy the same diagonal.

---

## 🗺️ Problem: Campus Navigation

Search algorithms are applied to a campus-navigation problem in which locations are represented as nodes and connections between locations are represented as edges.

The algorithms search for a path from a specified **start location** to a **goal location**.

The results can be used to observe differences between:

* BFS
* DFS
* Greedy Best-First Search
* A*
* Hill Climbing

---

## ♟️ Problem: N-Queens

The N-Queens problem demonstrates how AI can solve a constraint-based problem by systematically assigning values while satisfying the required constraints.

For example, for an `N × N` board:

```text
N = 4
```

one valid solution is:

```text
. Q . .
. . . Q
Q . . .
. . Q .
```

Here `Q` represents a queen and `.` represents an empty square.

---

## 📊 Search Strategy Comparison

| Algorithm         | Type         | Uses Heuristic | Complete | Optimal |
| ----------------- | ------------ | -------------- | -------- | ------- |
| BFS               | Uninformed   | ❌              | ✅        | ✅*      |
| DFS               | Uninformed   | ❌              | ⚠️       | ❌       |
| Greedy Best-First | Informed     | ✅              | ⚠️       | ❌       |
| A*                | Informed     | ✅              | ✅*       | ✅*      |
| Hill Climbing     | Local Search | ✅              | ❌        | ❌       |

`*` Depends on the problem conditions and assumptions.

---

## 🛠️ Technologies Used

* **Python**
* **Jupyter Notebook**
* Search algorithms
* Heuristic functions
* Constraint Satisfaction Problems

---

## 📁 Repository Structure

```text
Practical-Assignment-2-Problem-Solving-through-Search/
│
├── README.md
│
└── Practical Assignment 2 - Problem Solving through Search/
    │
    └── Campus_Navigation_and_N_Queens_AI_UPDATED.ipynb
```

---

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/ArshaDNakade/Practical-Assignment-2-Problem-Solving-through-Search.git
```

### 2. Navigate to the repository

```bash
cd Practical-Assignment-2-Problem-Solving-through-Search
```

### 3. Install Jupyter Notebook

```bash
pip install notebook
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Campus_Navigation_and_N_Queens_AI_UPDATED.ipynb
```

Run the cells sequentially to execute the practical.

---

## 📌 Expected Learning Outcomes

After completing this practical, the learner should be able to:

1. Explain problem-solving using search in Artificial Intelligence.
2. Implement BFS and DFS.
3. Understand informed search using heuristic functions.
4. Implement Greedy Best-First Search and A*.
5. Explain the difference between `g(n)`, `h(n)` and `f(n)`.
6. Understand the limitations of local search techniques such as Hill Climbing.
7. Formulate problems as Constraint Satisfaction Problems.
8. Solve the N-Queens problem using CSP techniques.
9. Compare different search strategies based on their behaviour and results.

---

## 👨‍💻 Author

**Arshad Nakade**

**Department:** Electronics & Telecommunication Engineering
**Program:** Third Year – Artificial Intelligence & Machine Learning / AI Practical

---

## 📚 Practical Assignment

**Practical Assignment 2: Problem Solving through Search**

This repository contains the implementation, execution, and results associated with the practical assignment.
