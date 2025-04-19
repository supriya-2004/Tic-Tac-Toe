# 🧩 Technology Stack Used

## 📄 HTML

- `<form>` - For player name inputs.
- `<input type="text">` - To capture Player 1 and Player 2 names.
- `<div class="board__cell">` - Represents individual game cells.
- `<div class="letter" data-id="0-8">` - Game state markers (`X` / `O`).
- `<button class="replay-btn">` - For resetting the game.

## 🎨 CSS

- `.board__container` - Holds the grid with `display: inline-block` and custom `box-shadow`.
- `.board__cell` - Styled for each Tic Tac Toe square.
- `.letter` - Holds the text (`X` / `O`) centered using `transform: translateY(-50%)`.
- `.input-field` & `.submit-btn` - Styled input and button with custom border and focus effects.
- `.hide-container` & `.reset--hidden` - Used to toggle visibility of form and board.

## ⚙️ JavaScript

- `window.addEventListener('load', app)` - Initializes the app.
- `addEventListener('submit', addPlayers)` - Captures player names.
- `addEventListener('click', resetBoard)` - Resets the board state.
- `gameBoard[]` - Tracks the current board state.
- `turn % 2 === 0 ? 'X' : 'O'` - Determines which player's turn.
- `document.querySelector("[data-id='0']")` - Used for selecting and updating specific cells.
- `winningSequences[]` - Logic array to check win conditions.
- `window.addEventListener("resize", onResize)` - Responsive square resizing logic.
