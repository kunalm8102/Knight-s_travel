# Knight's Travails Project

The goal of this project is to implement a function #knight_moves that shows the simplest possible way to get from one square to another using a Chess Knight.
The function will output all squares the knight will move to on its way. This is a variation on the [shortest path problem](https://en.wikipedia.org/wiki/Shortest_path_problem).

![Knight Possible Moves](/moves.gif)
![Knight Movement](/travails.gif)

![Screenshot](/knights_travails.png)


## Pre-Project Thoughts

1. This project lead me down the rabbit hole of Algorithms and Asymptotic Notation, which was my darkest yet.

2. I think I've gained a deeper knowledge of:

	1. Sorts, Implementation of Sorts, and Sort Efficiency
	2. Rudimentary Javascript
	3. Graphs: Vocabulary, Types, and the 3 Representations ,namely
		1. Edge Lists
		2. Adjacency Matrices
		3. Adjacency Lists
	4. Asymptotic Notation's Mathematical Proof
	5. Concept of Asymptotic Notation
		1. Big O Notation
		2. Big Θ Notation
		3. Big Ω Notation 


## Post-Project Thoughts

1.  I know that fully implementing Chess is only two projects away, I spent some extra time fleshing out class Gameboard so that it can handle properly presenting the game. I'm looking forward to getting started on that project as soon as possible.

2. The #knight_moves method was actually fairly easy to implement. First, I created a matrix of all existing positions. Then I performed a breadth-first search to fill an array 'distance_info' with each point's distance to the goal and their parent position. The breadth-first search continued until it reached the starting point. Then I iterated through the starting Knight's possible moves and selected the move that had the least distance from the goal position. This information was passed on to the display which moved the knight, and then searched for the next move until the full operation was complete.

4. Eventually, I may touch it up and add options for input. The user would be able to run the script and input a starting point and ending point. The script would then display the step-by-step moves from the starting to ending point. However, I know I will be fully implementing Chess shortly so I am eager to push forwards.

5. Apparently,I used [Dijkstra's Algorithm](https://en.wikipedia.org/wiki/Dijkstra%27s_algorithm) to find this solution.
