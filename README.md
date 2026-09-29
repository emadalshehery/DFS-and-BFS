# DFS and BFS

**Notebook:** `DFS_and_BFS.ipynb`

Two tree/graph traversal algorithms in Python, run on the same example tree.

## Tree

```
      A
     / \
    B   C
   / \   \
  D   E   F
```

Stored as an adjacency dictionary: `{'A': ['B','C'], 'B': ['D','E'], 'C': ['F'], 'D': set(), ...}`.

## Functions

| Function | Approach | Data structure |
|----------|----------|----------------|
| `bfs(tree, start)` | Level by level | `collections.deque` (queue) + `visited` set |
| `dfs(tree, start, visited=None)` | Goes deep first (recursive) | Call stack + `visited` set |

## Output

```
A B C D E F  BFS
A B D E C F  DFS
```

## Run

```bash
jupyter notebook DFS_and_BFS.ipynb
```

Only the Python standard library is needed.
