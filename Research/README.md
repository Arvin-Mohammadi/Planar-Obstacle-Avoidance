# Research Outline 

The main key points of this project are the following:
- Object Detection Algorithm
- Solving the Grid Problem
- Trajectory Generation

# Object Detection

I think I'll go with something like yolo-v5 default version for the moment because it's pretty easy to implement. 
I've already implemented the default model at [LINK](https://github.com/Arvin-Mohammadi/Autonomous-Vehicle-2021).

# Solving the Grid Problem

Assume that we have a grid-world with some obstacles, we can implement the [Breadth-First Search](https://www.geeksforgeeks.org/breadth-first-search-or-bfs-for-a-graph/) for finding the shortest path through the cells.

# Trajectory Generation 

I'll probably go for a point-to-point interpolating polynomial of 7th order. 
I've already solved the problem of trajectory generation for given points at [LINK](https://github.com/Arvin-Mohammadi/Delta-Robot-Trajectory-Planning-V3).

