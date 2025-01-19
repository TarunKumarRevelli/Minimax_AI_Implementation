# Connect Four AI Game

This is a Python implementation of the Connect Four game with an AI opponent. The AI uses the Minimax algorithm with alpha-beta pruning to make optimal moves.

## Features

- Two-player game: Player 1 (Human) vs Player 2 (AI).
- The game board is displayed using the Pygame library.
- AI uses a heuristic evaluation function to make strategic moves.
- Detects game-ending conditions: win (horizontal, vertical, diagonal) or draw.

---

## Prerequisites

- Python 3.x
- Pygame library

You can install Pygame by running:

```bash
pip install pygame
```

---

## How to Run

1. Save the script as `connect_four.py`.
2. Open a terminal or command prompt.
3. Run the script using the following command:

```bash
python connect_four.py
```

---

## How to Play

1. The game alternates between Player 1 and the AI.
2. Player 1 clicks on a column to drop a red piece.
3. The AI automatically makes its move (yellow piece).
4. The game ends when:
   - A player gets four consecutive pieces horizontally, vertically, or diagonally (win).
   - The board is full (draw).

---

## Key Functions

### 1. **Game Logic Functions**
- `create_board()`: Creates an empty Connect Four board.
- `drop_piece(board, row, col, piece)`: Drops a piece into the specified column.
- `is_valid_location(board, col)`: Checks if a column is valid for dropping a piece.
- `get_next_open_row(board, col)`: Gets the next available row in the specified column.
- `winning_move(board, piece)`: Checks if the given piece has achieved a winning position.

### 2. **AI Functions**
- `evaluate_board(board, piece)`: Evaluates the board's heuristic score for the given piece.
- `evaluate_window(window, piece)`: Evaluates a window of 4 cells based on the number of pieces and empty spaces.
- `minimax(board, depth, alpha, beta, maximizing_player, piece)`: Implements the Minimax algorithm with alpha-beta pruning to find the best move for the AI.

### 3. **Pygame Functions**
- `draw_board(board)`: Draws the Connect Four board using Pygame.

---

## Game Board Dimensions

- **Rows**: 6
- **Columns**: 7
- **Square Size**: 100px

---

## Colors Used

- **Blue**: Board background
- **Black**: Empty slots
- **Red**: Player 1 pieces
- **Yellow**: AI pieces

---

## Example Gameplay

1. Run the game, and the empty board will be displayed.
2. Player 1 clicks on the desired column to drop their piece.
3. The AI calculates its move and places its piece.
4. The game continues until there is a winner or a draw.

---

## Future Improvements

- Add difficulty levels for the AI.
- Implement animations for piece drops.
- Create a scoreboard to track multiple rounds.

---

## Author

This implementation was created for educational purposes, showcasing how to combine Python game development with basic AI techniques.

