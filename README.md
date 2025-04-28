## Features

### Core Functionality

#### **Game Mechanics:**
- Interactive chessboard implemented using `ChessBoard`, `ChessWindow`, and `MainWindow` classes.
- Move generation and validation using internal logic, assisted by Stockfish.
- Game states tracked and updated automatically after every move.
- Support for special moves:
  - Castling
  - En passant
  - Pawn promotion

#### **Stockfish Integration:**
- Communicates with the Stockfish engine via the `StockfishConnector` class.
- Retrieves:
  - Best moves
  - Evaluation scores
  - List of legal moves
- Adjustable:
  - Search depth
  - Move time per turn
  - Number of search threads for performance tuning

#### **Move Storage and Analysis:**
- Tracks full move history internally using `ChessGame`.
- Sends move sequences to Stockfish for accurate position evaluation.
- Supports dynamic engine updates during live gameplay.

---

### User Interface

#### **JavaFX-Based GUI:**
- Visual representation of the chessboard and pieces using `ChessWindow` and `MainWindow`.
- Drag-and-drop functionality for natural piece movement.
- Real-time board updates after moves, captures, castling, and promotions.
- Clean and responsive user interface with custom graphics.

#### **Scalable Design:**
- Modular architecture for easy extension and maintenance.
- Clear separation of concerns:
  - Game logic (`ChessBoard`, `ChessGame`)
  - UI rendering (`ChessWindow`, `MainWindow`)
  - Engine communication (`StockfishConnector`)
- Designed for future upgrades, including stronger AI integration or advanced analysis tools.
