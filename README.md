# Flight Route Optimization: Shortest Path Analysis

## 📌 Project Overview
This project implements and compares two fundamental graph algorithms—**Dijkstra** and **Bellman-Ford**—to solve the shortest path problem. Using a dataset of 2,000 flight records, the system identifies the most efficient routes between 268 US airports.

## 🛠️ Implementation Details
- **Language:** Python
- **Environment:** Kaggle / Jupyter Notebook
- **Dataset:** [2015 Flight Delays and Cancellations](https://www.kaggle.com/usdot/flight-delays)

## 📊 Algorithm Comparison

| Feature | Dijkstra's Algorithm | Bellman-Ford Algorithm |
| :--- | :--- | :--- |
| **Design Family** | Greedy | Dynamic Programming |
| **Complexity (Avg)** | O((V + E) log V) | O(V * E) |
| **Use Case** | Positive weights, high speed |
| **Observed Time** | **31.45 ms** | **2.1** |

## 📈 Analysis (Best, Average, Worst Case)
### Dijkstra
- **Best Case:** Ω(V + E) - Occurs when the graph is sparse or the destination is found early.
- **Average Case:** Θ((V + E) log V) - The typical performance seen in our flight mapping.
- **Worst Case:** O((V + E) log V) - When every airport is connected to every other airport.

### Bellman-Ford
- **Best Case:** Ω(E) - Occurs if the graph is already relaxed.
- **Average/Worst Case:** O(V * E) - Necessary when checking for all possible edge relaxations over V-1 iterations.
