# A-star-search-algorithm
This is an A star search algorithm with graph search implemented to plan a robots path


## Problem description
The inputs to your program are the start and goal positions of a point robot, and a 2D integer array that represents the robot workspace. The robot can move from cell to cell in any of the eight directions. The goal is to find the lowest-cost path between the start position and the goal position, and avoiding obstacles along the path. The workspace is represented as an occupancy grid, where the black cells represent obstacles.
![Sample workspace of the robot with an unoptimal path in red.](assets/images/Sample_workspace.png)


## Defining costs of each step to find an optimal path

Let each cell in the workspace be a state. Therefore white cells are legal states(the robot is allowed to move to that cell) and black cells are illegal states(the cell is an obstacle). Each step cost can be calculated by the sum of angle cost(change of angle in movement from the previous step) and distance cost. 
Distance cost is easy to determine wherein the distance cost for horizontal and vertical moves is 1 and $\sqrt{2} for diagnol moves.
