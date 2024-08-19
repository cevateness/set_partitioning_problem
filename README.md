# Set Partitioning Problem (SPP) Solver

This repository contains various implementations for solving the Set Partitioning Problem (SPP), a combinatorial optimization problem often found in scheduling, crew assignment, and routing applications. The repo explores different methods ranging from exact algorithms to constraint programming and heuristic techniques.

## Problem Description

The Set Partitioning Problem (SPP) is defined as follows:

- **Input:** A set of elements and a collection of subsets, each associated with a cost.
- **Objective:** Select a collection of subsets such that:
  - Each element is covered exactly once.
  - The total cost of the selected subsets is minimized.

### Example Problem
Given elements `{1, 2, 3, 4, 5, 6}`, and the following subsets with associated costs:
- Subset 1: `{1, 2}` with cost 4
- Subset 2: `{2, 3, 4}` with cost 6
- Subset 3: `{3, 5}` with cost 5
- Subset 4: `{4, 6}` with cost 7
- Subset 5: `{5, 6}` with cost 3

The goal is to select subsets that cover all elements exactly once, while minimizing the total cost.

## Implemented Methods

This repository includes multiple approaches for solving the SPP:

1. **Brute-Force Search:**
   - Explores all possible combinations to find the optimal solution. Suitable for small-scale problems.

2. **Branch and Bound:**
   - Uses a tree structure to explore feasible solutions while pruning branches that cannot yield better results.

3. **Constraint Programming (CP) with Google OR-Tools:**
   - Leverages the CP-SAT solver to efficiently handle logical constraints and find an optimal solution.

4. **Metaheuristics (Future Implementation):**
   - Planned integration of Genetic Algorithms, Simulated Annealing, and Tabu Search for large problem instances.

5. **Gurobi Integration:**
   - Provides a comparison using the Gurobi solver for Mixed-Integer Programming (MIP).


