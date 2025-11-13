# Quick Reference Guide - Graph Algorithms

## 🚀 Quick Start

```
# Activate environment
.\venv\Scripts\Activate.ps1

# Open notebook
jupyter notebook graph_realworld.ipynb

# Run all cells: Ctrl+A → Shift+Enter
```

## 📊 Algorithms At A Glance

### 1️⃣ BFS/DFS (Social Network)
```
Time: O(V + E) | Space: O(V)
Use: Finding connected components, friends
Data Structure: Queue (BFS) or Stack (DFS)
```

### 2️⃣ Bellman-Ford (Google Maps)
```
Time: O(V × E) | Space: O(V)
Use: Shortest paths with negative weights
Detects: Negative cycles
Best: Small graphs, negative weights needed
```

### 3️⃣ Dijkstra's (Emergency Response)
```
Time: O(E log V) | Space: O(V)
Use: Shortest paths, all positive weights
Data Structure: Min-heap / Priority queue
Best: Large graphs, GPS navigation
```

### 4️⃣ Prim's MST (Cable Installation)
```
Time: O(E log V) | Space: O(V + E)
Use: Minimum spanning trees
Alternative: Kruskal's with Union-Find
Best: Network design, infrastructure
```

## 🧪 Test Results

| Algorithm | Problem | Result | Status |
|-----------|---------|--------|--------|
| BFS | Friends for A | ['E', 'F', 'D'] | ✓ |
| Bellman-Ford | Path from 0 | {0:0, 1:5, 2:2, 3:7, 4:4} | ✓ |
| Dijkstra's | Route to F | 13 units | ✓ |
| Prim's MST | Cable cost | 10 units | ✓ |

## 📁 Project Structure

```
Your Project Folder/
│
├── graph_realworld.ipynb     ← Main submission
├── README.md                  ← Setup guide
├── requirements.txt           ← Dependencies
├── SUBMISSION.md              ← Checklist
├── QUICK_REFERENCE.md         ← This file
├── .gitignore
└── venv/                      ← Virtual environment
```

## ⚡ Common Commands

```
# Update requirements
pip freeze > requirements.txt

# Install from requirements
pip install -r requirements.txt

# Check installed packages
pip list

# Run notebook
jupyter notebook

# Deactivate environment
deactivate
```

## 🎯 Complexity Comparison

```
               Small (< 50)  Medium (50-500)  Large (> 500)
BFS/DFS        ✓✓ Instant   ✓ Fast           ✓ Good
Bellman-Ford   ✓ Fast       ⚠ Slow           ✗ Very slow
Dijkstra's     ✓✓ Instant   ✓✓ Fast          ✓ Good
MST (Prim's)   ✓✓ Instant   ✓✓ Fast          ✓ Good
```

## 📝 Key Takeaways

1. **Choose algorithm** based on problem constraints
2. **Time complexity** matters for large datasets
3. **Space complexity** important for memory-limited systems
4. **Profile before optimizing** - theory ≠ practice
5. **Data structures** (heap, queue, set) impact performance

---

**Last Updated:** November 3, 2025 | **Status:** Complete ✅