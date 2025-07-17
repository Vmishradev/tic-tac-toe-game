# Tic-Tac-Toe Game

A classic Tic-Tac-Toe game built with React, featuring an interactive game board, move history, and time travel functionality.

## Features

- **Interactive Game Board**: Click on squares to make your move
- **Two-Player Gameplay**: Alternates between X and O players
- **Winner Detection**: Automatically detects winning combinations
- **Game History**: Keep track of all moves made during the game
- **Time Travel**: Jump back to any previous move in the game
- **Clean UI**: Simple and intuitive user interface

## Game Rules

1. The game is played on a 3x3 grid
2. Players take turns placing their mark (X or O) in empty squares
3. The first player to get 3 marks in a row (horizontally, vertically, or diagonally) wins
4. If all squares are filled and no player has won, the game ends in a draw

## Technology Stack

- **React**: Frontend framework with hooks (useState)
- **CSS**: Styling for the game interface
- **JavaScript**: Game logic and state management

## Project Structure

```
TIC-TAC-TOE-GAME/
├── node_modules/
├── public/
│   ├── favicon.ico
│   ├── index.html
│   ├── logo192.png
│   ├── logo512.png
│   ├── manifest.json
│   └── robots.txt
├── src/
│   ├── App.css
│   ├── App.js
│   ├── App.test.js
│   ├── index.css
│   ├── index.js
│   ├── logo.svg
│   ├── reportWebVitals.js
│   └── setupTests.js
├── .gitignore
├── package-lock.json
├── package.json
└── README.md
```

## Installation

1. **Clone the repository**
   ```bash
   git clone [<repository-url>](https://github.com/Vmishradev/tic-tac-toe-game)
   cd TIC-TAC-TOE-GAME
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```

4. **Open your browser**
   Navigate to `http://localhost:3000` to play the game

## Available Scripts

- `npm start` - Runs the app in development mode
- `npm test` - Launches the test runner
- `npm run build` - Builds the app for production
- `npm run eject` - Ejects from Create React App (one-way operation)

## Component Architecture

### Main Components

1. **Game Component**: 
   - Root component managing game state
   - Handles move history and time travel functionality
   - Renders the game board and move list

2. **Board Component**:
   - Manages the current game state
   - Handles player moves and winner detection
   - Renders the 3x3 grid of squares

3. **Square Component**:
   - Individual clickable square
   - Displays X, O, or empty state
   - Handles click events

### Key Functions

- `calculateWinner()`: Checks for winning combinations
- `handleClick()`: Processes square clicks and updates game state
- `handlePlay()`: Manages move history
- `jumpTo()`: Enables time travel to previous moves

## Game Flow

1. Game starts with an empty 3x3 board
2. Player X goes first
3. Players alternate turns by clicking empty squares
4. Game detects winner or draw condition
5. Players can review move history and jump to previous states

## Winning Conditions

The game checks for wins in:
- **Rows**: [0,1,2], [3,4,5], [6,7,8]
- **Columns**: [0,3,6], [1,4,7], [2,5,8]
- **Diagonals**: [0,4,8], [2,4,6]

## Future Enhancements

- Add player name customization
- Implement score tracking across multiple games
- Add AI opponent with difficulty levels
- Include sound effects and animations
- Add responsive design for mobile devices
- Implement online multiplayer functionality

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

## Acknowledgments

- Built following React's official tutorial
- Inspired by the classic Tic-Tac-Toe game
- Uses Create React App for quick setup and development
