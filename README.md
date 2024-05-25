# Tic Tac Toe AI Game

## Description

This project is a Tic Tac Toe game with a graphical user interface (GUI) created using Pygame. It allows a user to play against an AI opponent. The AI uses the minimax algorithm with alpha-beta pruning to make optimal moves.

## Installation

1. **Clone the Repository:**

   ```sh
   git clone https://github.com/yourusername/tictactoe-ai.git
   cd tictactoe-ai
   ```

2. **Install the Required Packages:**

   Ensure you have Python and Pygame installed. You can install Pygame using pip:

   ```sh
   pip install pygame
   ```

3. **Download Fonts:**

   Download the `OpenSans-Regular.ttf` font and place it in the project directory.

## Usage

1. **Run the Game:**

   To start the game, run the `runner.py` script:

   ```sh
   python runner.py
   ```

2. **Playing the Game:**

   - When the game starts, choose to play as either X or O by clicking the respective button.
   - The game board will be displayed, and you can make moves by clicking on the empty cells.
   - The AI will automatically make its move after you.
   - The game will display the winner or indicate a tie when the game is over.
   - Click the "Play Again" button to start a new game.

## Game Rules

- The game is played on a 3x3 grid.
- Players take turns placing their mark (X or O) in an empty cell.
- The first player to get three of their marks in a row (horizontally, vertically, or diagonally) wins.
- If all nine cells are filled without a winner, the game ends in a tie.



## Files

- `runner.py`: The main script that runs the game with a Pygame GUI.
- `tictactoe.py`: Contains the main functions of the game, including the minimax algorithm for the AI.

## Main Functions (from `tictactoe.py`)

- `initial_state()`: Returns the starting state of the board.
- `player(board)`: Returns the player who has the next turn on a board.
- `actions(board)`: Returns a set of all possible actions available on the board.
- `result(board, action)`: Returns the board that results from making a move.
- `winner(board)`: Returns the winner of the game, if there is one.
- `terminal(board)`: Returns True if the game is over, False otherwise.
- `utility(board)`: Returns 1 if X has won, -1 if O has won, 0 otherwise.
- `minimax(board)`: Returns the optimal action for the current player on the board.
