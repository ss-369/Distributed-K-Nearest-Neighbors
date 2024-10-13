
---

### 1. **Distributed K-Nearest Neighbors**

# Distributed K-Nearest Neighbors

## Description

This program implements a distributed solution for the **K-Nearest Neighbors** algorithm using MPI. The program finds the **K nearest neighbors** of each query point from a set of points in a 2D plane based on Euclidean distance.

## Requirements

- **Language**: C/C++ (recommended), Python
- **Framework**: MPI

## Input Format

- The first line contains three integers, `N` (number of points in set P), `M` (number of query points in set Q), and `K` (number of nearest neighbors to find).
- The next `N` lines contain two space-separated floating-point numbers, representing the coordinates of points in set P.
- The following `M` lines contain two space-separated floating-point numbers, representing the coordinates of query points in set Q.

## Output Format

- For each query, print the coordinates of its `K` nearest neighbors (one per line).

## Example

### Input
```
5 3 2
0.12 34
42 1.24
5 -78.4
21.72 -18.76
61.45 74.9
21.41 34.34
-1.47 63.3
41.3 -6
```

### Output
```
0.12 34
42 1.24
0.12 34
61.45 74.9
42 1.24
21.72 -18.76
```

## How to Run

1. Compile the program:
   ```bash
   mpicc -o knn 1.cpp
   ```

2. Run the program with MPI:
   ```bash
   mpiexec -np <number_of_processes> ./knn <input_file>
   ```

---

