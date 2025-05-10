### Balanced Graph Generator


### Description
This script balances a directed graph by adjusting the number of outgoing and incoming edges per node. It calculates the difference between in-degree and out-degree for each node and attempts to balance the graph by adding edges accordingly. The goal is to prepare a graph structure suitable for algorithms that require balanced graphs, such as Eulerian path or circuit algorithms.

### Usage

Example Input:

```
graph_input = {
    1: [2, 3, 5],
    2: [1, 4],
    3: [2, 5],
    4: [1, 2, 5],
    5: [3, 4]
}
```

Run:
```
balanced_graph = balance_graph(graph_input)

for node, neighbors in balanced_graph.items():
    print(f"{node} -> {neighbors}")
``` 
### Applications
* This function has several use cases in computational graph theory and bioinformatics:
* Eulerian Path Preparation: Prepares graphs to satisfy the in-degree = out-degree condition required for finding Eulerian circuits or paths.
* Synthetic Graph Construction: Helps in generating graph datasets with controlled balance.
* Network Flow Simulations: Useful in network analysis where equilibrium of input/output connections is essential.
* Genome Assembly: Assists in balancing de Bruijn graphs prior to traversing them for sequence reconstruction.

### License
This project is licensed under the MIT License.
