# Shatranj-AI
A Chess Engine which rely on the powers of Computation and Game Theory.

## About
Shatranj-AI is a simple chess AI in JavaScript.

The primary concern of Shatranj-AI is the decision-making part of the application. All functionality outside the scope of the AI are implemented using external libraries:
- Chessboard GUI: Using the chessboard.js API
- Game Mechanics: Using the chess.js API

The AI uses the [minimax algorithm](https://en.wikipedia.org/wiki/Minimax), which is optimised by [alpha-beta pruning](https://en.wikipedia.org/wiki/Alpha%E2%80%93beta_pruning). 

The evaluation function uses [piece square tables](https://www.chessprogramming.org/Piece-Square_Tables) adapted from Sunfish.py, and eliminates the need for nested loops by updating the sum based on each move instead of re-computing the sum of individual pieces at each leaf node.

A global sum is used to keep track of black's evaluation score after each move, which is used to display the 'advantage' bar. 

## Thanks

Special thanks to these projects that help me a lot in this.
1. [Chess.js](https://github.com/jhlywa/chess.js)
2. [Chessboard.js](https://chessboardjs.com)
3. [Free Code Camp](https://www.freecodecamp.org/news/simple-chess-ai-step-by-step-1d55a9266977/)
