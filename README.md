# Mancala

Mancala is an ancient board game where two players take turns moving stones between pockets on a board. By following specific rules, players distribute their stones counterclockwise, aiming to capture the opponent's pieces and collect as many stones as possible in their own Mancala store. The game continues until one player runs out of stones, and the winner is determined by the number of stones in their Mancala store.

Mancala tutorial: https://youtu.be/-A-djjimCcM

## How to Run

You can choose to run two AI agents against one another via the Mancala GUI or play against an the AI yourself. Running the code will bring up a game window. Each agent will alternate turns.

The GUI takes two AI programs as parameters for instance:
```
> python3 mancala_gui.py -d 5 -a agent.py -b randy_ai.py 
```

Play against an AI by specify only one player:
```
> python3 mancala_gui.py -d 5 -a agent.py -t 1 -l 6
```
The arguments supplied are as follows:
* -h: for help
* -d: for the dimension of the board (i.e. the # of pockets)
* -a: the first player
* -b: the second player
* -c: for state caching
* -l: for the depth limit
* -t: for the type of agent, which can be 0 (minimax), 1 (alpha-beta) or 2 (mcts)
