<a name="graph"></a>
# Graph
We use `T.Graph` in `t.graph.js` to help implementations of some algorithms in `Graph` static object, which has been put in `graph.*.js`.

All the following methods are invoked like `Graph.*`. To create a graph object, use `new T.Graph*()` (see [APIType](APIType#graph)).

#### `bfs(graph): []`
Gets the vertex visiting array by BFS order.
#### `dfs(graph): []`
Gets the vertex visiting array by DFS order.
#### `dijkstra(graph, s: number = 1): []`
Gets the shortest path length of each vertex from initial vertex $s$.
#### `multiMinimumCut(graph, times: number): number`
Gets the minimum cut number of graph after that times calculations.
#### `mstPrim(graph, s: number = 1): number`
Gets the total MST cost of weighted graph by Prim algorithm.
#### `mstKruskal(graph): number`
Gets the total MST cost of weighted graph by Kruskal algorithm.
#### `mstKruskal(graph, k): number`
Gets the max space of k-clustering by Kruskal algorithm.
#### `sccKosaraju(graph): []`
Gets the top $10$ large size strong connect component of directed graph, using Kosaraju algorithm.
#### `topologicalSort(graph): []`
Gets the topological visiting array of this directed graph.
#### `undirectedConnected(graph): []`
Gets an array indicating connectivity info of undirected graph. this undirected graph is connected iff  `result.length == 1` AND `result[0][1] == Graph.dfs(graph)`.

[Back to top](#graph)