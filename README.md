Overview
This is a simplified implementation of the classic Minesweeper game in C++. The program simulates a minefield where the player can reveal cells or flag potential mines. It uses fixed dimensions for the minefield and avoids arrays, making it suitable for beginner-level programming.

Features
Fixed Minefield Size: The board is 5 columns wide and 8 rows tall.
Game States:
Cells can be flagged, revealed, or remain unknown.
The game tracks correct and incorrect flags and handles mine explosions.
Random Mine Placement: Mines are randomly distributed across the field.
Modular Design: Functions are used for specific tasks, making the program easy to read and expand.
How It Works
Cell States
Each cell can have one of the following states:

UNKNOWN (-4): Default state; the cell hasn't been revealed or flagged.
UNFLAGGED_MINE (-1): The cell contains a mine but hasn’t been flagged.
FLAGGED_MINE (-2): The cell has been correctly flagged as a mine.
INCORRECT_FLAGGED_MINE (-3): The cell was flagged but does not contain a mine.
Number (0–8): Revealed cells show the number of adjacent mines.
Game Progress
The game progresses until:

The player correctly flags all mines without triggering one.
A mine explodes, ending the game.
