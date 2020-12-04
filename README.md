# IS 597: DSO
# Welcome to my fork of project 'AI' by author - github user ID: tochinton</br>
# This is a submission for IS 597: DSO</br>
## TYPE 3 Solved Game Analysis on Hexapawn

This is a game of hexapawn. I have used and modified the original code by tochiton to prove that Hexapawn is a solved game for my analysis. I have also included variations to play the 4X4 version and also a 5X5 version of the game, for the purpose of this analysis. This program uses minimax and alpha beta pruning for the game tree search and move selection.

# Motivation behind the project
I was very intrigued by the concept of “solved games”, perfect information and perfect play. That is why I chose to select this topic for my final project. For me, as the aim of the project, grasping and demonstrating the concept computationally was more important than the game I selected to demonstrate that. I have to say I thouroughly enjoyed the process and learned so much along the way. 

# How to run:
For the purposes of this project, you only need to run the file "main.py". It is the file that I have worked on.</br>
Once you run it, you will bw given the option to play a game of 3X3, 4X4 or 5X5 pawn game. It is totally upto you to select which one you would like to select. I would recommend playing with the 3X3 version first to understand the concept thoroughly before moving on to the 4X4 version and so on. Even though the board could be of size nXm, I have selected these 3 sizes for the purpose of my analysis. 

# Outcomes and Findings:
My aim is to prove that hexapawn is a weakly solved game and here I will try to demonstrate how, with the help of an example:
Here you can see that after White(human player) makes the move, the first move in this case, Black pawn(bot) is "thinking". It explores all the 3 possible moves, and digs deeper to the depth of a selected move. It looks ahead upto 2 moves. At this point, you can see that whatever you do, black wins. Black makes a move. Neverthless, player plays and the very next move black moves is a winning move.
Here are two ways, a screenshot and game tree of what I am trying to explain. The game tree is specific to another sequence of moves, which also ensures a win for black.
Hence, no matter what the player does, black always wins. Hexapawn has a first player disadvantage.

![Screenshot](ss1.png)
![Screenshot](ss2.png)

## 4X4 Variant
In this type of variant, no matter what, second player always loses.

## Original Read.me from the author
tested on python 2.7
run AI using: python main.py

let’s formally define steps of the algorithm:

Construct the complete game tree
Evaluate scores for leaves using the evaluation function
Back-up scores from leaves to root, considering the player type:
For max player, select the child with the maximum score
For min player, select the child with the minimum score
At the root node, choose the node with max value and perform the corresponding move


