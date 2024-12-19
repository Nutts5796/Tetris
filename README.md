Tetris Game in C

This is a simple implementation of the classic Tetris game written in C. The project is designed to provide a smooth, playable experience and includes the core functionality of the game, such as piece movement, rotation, line clearing, and collision detection. The game uses a custom data structure to represent the game field, Tetromino pieces, and the state of the game.

Features
    •    Field Representation: The game field is represented as a 2D array, with blocks stored in each cell.
    •    Tetrominoes: Various Tetromino pieces (T, I, O, L, J, Z, and S shapes) are handled, and each has its own rotation logic.
    •    Piece Movement: Players can move pieces left, right, down, or rotate them.
    •    Collision Detection: Prevents pieces from moving into filled areas or out of bounds.
    •    Line Clearing: Automatically clears filled lines and updates the score accordingly.
    •    Game Over: The game ends when a new piece cannot be placed on the field due to collisions.
    •    Score Tracking: The score increases as lines are cleared, providing feedback to the player.

Structure

The game is built with the following components:
    •    TetField: A structure that holds the current game field, representing the grid where Tetromino pieces are placed.
    •    TetFiguresT: Stores the available Tetromino pieces and their properties.
    •    TetGame: Manages the overall game state, including the field, active pieces, and score.
    •    TetFigure: Represents the current active Tetromino, including its position, rotation, and the blocks that form it.

Functions
    •    createTetField: Initializes the game field with a specified width and height.
    •    createTetFiguresT: Initializes the Tetrominoes, specifying the number of pieces and their sizes.
    •    moveFigureLeft/Right/Down: Functions that move the active Tetromino in the respective direction.
    •    collisionTet: Checks if the current piece collides with other pieces or the boundaries.
    •    plantFigure: Places the current Tetromino on the field.
    •    eraseLinesTet: Clears filled lines from the field and updates the score.
    •    dropNewFigure: Spawns a new Tetromino at the top of the screen.
    •    rotTetFigure: Rotates the current Tetromino.

How to Play
    • Move pieces using the A (left), D (right), and S (down) keys.
    • Rotate pieces using the W key.
    • The game will automatically drop pieces over time, and you need to position them to form complete horizontal lines.
    • The game ends when a piece can’t be placed at the top of the screen.
    • Your score increases as you clear lines.
