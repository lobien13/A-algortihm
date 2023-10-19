# A-algortihm

The A* (A Star) algorithm is a widely used heuristic search algorithm for solving pathfinding problems in fields such as artificial intelligence, robotics, and video games. A* is particularly effective at finding the shortest path between two points in a graph or map. Its popularity stems from its efficiency and ability to find optimal solutions.
The A* algorithm operates using a graph search approach, where nodes are evaluated and expanded to find the shortest path from a starting node to a destination node. A* combines two key components to achieve this: the actual cost from the starting node to the current node (g) and a heuristic estimate of the cost from the current node to the destination node (h). The total cost f is the sum of these two values: f = g + h.

The algorithm proceeds as follows:

Initialize two sets, one for open nodes and one for closed nodes.
Add the starting node to the open node set.
While the open node set is not empty:
a. Select the node with the lowest f value from the open node set.
b. Move this node from the open node set to the closed node set.
c. Expand the selected node, generating successor nodes and computing their f, g, and h values.
d. For each successor:
If it is in the closed node set, ignore it.
If it is not in the open node set, add it.
If it is already in the open node set and the new g value is lower, update the g value and recalculate f.
When the destination node is found or the open node set is empty, the search terminates.

