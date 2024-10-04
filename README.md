# flip-solver
A solver for the Flip game, as on Simon Tatham's Puzzles website (this game is also known as Lights Out).

This solver is implemented in Sage, which is a wrapper around Python.

## Example Usage
The following is done in a Sage repl started in the root of this repo.
```sage
> load("flip.sage")
> game_link = "https://www.chiark.greenend.org.uk/~sgtatham/puzzles/js/flip.html#5x5:c600007080001c4000070800018c000631000318400043080009c0000c2100018c000007280001c4000470000118800043100009c800007200000ce00042300018c000027000009c0000270000318,716a020"
> solve_game_link(game_link)
[0 1 1 0 0]
[1 0 1 0 0]
[1 0 1 1 1]
[1 1 0 1 1]
[0 0 0 0 0]
```
The output is a matrix of the same dimensions as the board of the game. A 1 in the output indicates that you should click that cell.
