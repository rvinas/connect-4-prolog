# Connect 4 Prolog
## Description
Connect 4 is a two player board game that takes place in a 6x7 grid. Players alternatively drop their discs into one of the 7 columns of the grid.
A column is always filled up from bottom to top. The player who achieves the connection of 4 discs (horizontally, vertically or diagonally) wins the game.
The game ends up in a draw when the grid is full without any straight connection of 4 discs from a single player.

This repository is intended to serve as an exercise to learn Prolog. We implement the Connect 4 game providing a naive machine player, which tries to achieve the following goals within a single depth level (priority decreases from top to bottom items):
* Win within a movement.
* Intercept a 4-connection from the opponent, placing the disc in a spot that increases a machine's connection.
* Intercept a 4-connection from the opponent.
* Play arbitrarily. By default, it drags the disc in the first free spot from left to right columns.

## Requirements
We recommend using the GNU Prolog Compiler ([gprolog](http://www.gprolog.org/)) developed by Daniel Diaz. Once gprolog is installed, the steps to run the game are straightforward:
* Execute `gprolog` in command line.
* Once in gprolog environment, compile with `[connect4].`.
* Finally, run game with `connect4.`. Enter a character from A to G to drop a disc down to the associated column.

It may also work with other compilers, although we haven't tested them.

## Further improvements
We leave the following items as open improvements:
* Develop an Artificial Intelligence for the game in Prolog.
* Develop a user interface.
