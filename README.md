# Tic-Tac-Toe Game with Alpha-Beta Pruning in Python

This project is a **Tic-Tac-Toe game** built using Python's **Tkinter** library for the GUI and an **Alpha-Beta pruning algorithm** to enable an AI opponent. The game offers both single-player and two-player modes and is designed for an enjoyable user experience with intuitive controls.

## Features

- **Play against the computer or a friend**: Choose between single-player mode, where the computer uses the Alpha-Beta algorithm, or two-player mode.
- **Intelligent AI with Alpha-Beta Pruning**: The computer player utilizes Alpha-Beta pruning for optimal gameplay.
- **Graphical Interface**: Built using Tkinter for a smooth, visually appealing experience.
- **Play Again and Reset Options**: Easily reset or start a new game after each round.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/tic-tac-toe-alpha-beta.git
   cd tic-tac-toe-alpha-beta
   ```

2. **Install dependencies** (only requires Tkinter, which comes pre-installed with Python):
   ```bash
   pip install tk
   ```

3. **Run the game**:
   ```bash
   python tic_tac_toe.py
   ```

# Game Controls

- **Play Button**: On startup, click "Play" to enter the game menu.
- **Select Mode**: Choose "Play with Computer" or "Play with Friend."
- **Reset Button**: Available during gameplay to reset the board.
- **Back Button**: Return to the main menu at any time.

# Code Overview

# `AlphaBeta` Class
This class is responsible for implementing the Alpha-Beta pruning algorithm, which allows the computer to make optimal moves.

-### Key Methods**:
  - `is_terminal(state)`: Checks if the current game state has a winner or if it’s a draw.
  - `utility(state)`: Evaluates the game state, returning a score based on the winner.
  - `alpha_beta(...)`: Recursively calculates the best move for the computer, minimizing the search space through Alpha-Beta pruning.
  - `best_move(state)`: Determines the best possible move based on current game state.

# `TicTacToeGUI` Class
This class builds the Tkinter graphical interface, handles player interactions, and manages game flow.

- ### Key Functionalities:
  - **Game Menu**: Allows players to select between single-player and two-player modes.
  - **Game Board**: Displays a 3x3 grid for Tic-Tac-Toe.
  - **Move Handling**: Alternates turns between players or computer.
  - **Win Checking and Messaging**: Displays a pop-up message for win/loss/draw results and resets the board.

#Example Gameplay

On launch, you’ll see the "Play" button. After selecting a mode, a 3x3 grid will appear. Player O typically goes first. In single-player mode, the computer plays as X, attempting to win or block the player using the Alpha-Beta pruning strategy.
