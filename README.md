Student:Tomiris Chekalin
Group:It-2503

Class Description:


Vertices Class:


Represents a node in the graph.


 Methods that in my code:
 
  
Constructor
Getter
toString() 

Edge Class:


Represents a connection between two vertices.id — unique identifier


  Fields
-source
-destination

  Methods  

  
Constructor
Getters
toString()

Graph Class:


Represents the graph structure using adjacency lists.

Main Methods



addVertex(Vertex v)
addEdge(int from, int to)
printGraph()
bfs(int start)
dfs(int start)

Experiment Class:


Handles graph experiments and performance analysis.

Methods


runTraversals(Graph g)
runMultipleTests()
printResults()



Algorithm Descriptions:


1)Breadth-First Search visits graph nodes level by level.BFS uses a Queue data structure.



BFS Step by step:





1.Start from a node.2.Visit all neighboring nodes.3.Add neighbors to queue.4.Continue until queue becomes empty


BFS use cases:





1.Shortest path in unweighted graph.2.Network broadcasting.3.GPS systems.4.Web crawling.





BFS Time Complexity:O(V + E)

Where:V = vertices,E = edges 





2)Depth-First Search (DFS)

Depth-First Search explores graph nodes deeply before backtracking.DFS uses Recursion or Stack.





DFS Step by step:
1.Visit current node.2.Move to unvisited neighbor.3.Continue deeper.4.Backtrack if necessary





DFS Use Cases:
1.Path finding.2.Cycle detection.3.Maze solving4.Topological sorting





DFS Time Complexity:O(V + E)



Where:V = vertices,E = edges

  

Experimental Results:


[screenshots.docx](https://github.com/user-attachments/files/27517921/screenshots.docx)





Larger graphs require more traversal time.
BFS and DFS both showed linear growth.
Results match expected complexity O(V + E).
BFS was slightly faster in some experiments.
Traversal order changes depending on graph structure.






BFS                      	DFS
Uses Queue              	Uses Stack/Recursion
Level-by-level traversal	Deep traversal
Better for shortest path	Better for deep exploration
Higher memory usage     	Lower memory usage  




Analysis Questions:


How does graph size affect BFS and DFS performance?
As the number of vertices and edges increases, traversal time also increases because more nodes must be visited.



Which traversal is faster in your experiments?
BFS was slightly faster in small graphs, but both algorithms showed similar performance.



Do results match expected complexity O(V + E)?
Yes. Both BFS and DFS visit each vertex and edge once.



How does graph structure affect traversal order?
Different edge connections produce different traversal paths and visiting order.



When is BFS preferred over DFS?
BFS is preferred when finding the shortest path in an unweighted graph.



What are the limitations of DFS?
DFS may go very deep into the graph and can consume stack memory because of recursion.



Reflection
In this assignment I learned how graphs work and how traversal algorithms operate. I understood the difference between BFS and DFS and how adjacency lists store graph data efficiently.
The biggest challenge was implementing traversal logic correctly and understanding recursion in DFS. I also learned how execution time changes depending on graph size and structure.



Conclusion
This project successfully demonstrates graph representation and traversal algorithms using Java. BFS and DFS are important algorithms used in many real-world systems such as navigation, social networks, and search engines.

