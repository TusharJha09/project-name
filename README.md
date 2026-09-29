# 🐍 Snake & Ladder Game

A **responsive browser-based Snake & Ladder game** built using **HTML, CSS, and JavaScript**. The project recreates the classic two-player board game with an interactive 10×10 game board, dice-based movement, snakes, ladders, turn management, winner detection, and game restart functionality.

The application is designed as a simple frontend project that demonstrates how **JavaScript can be used to manage game logic, dynamically generate HTML elements, update the user interface, and handle user interactions**.

## 🚀 Features

* 🎲 **Interactive Dice Rolling**

  * Generates a random dice value from 1 to 6.
  * Displays the corresponding dice face using Unicode symbols.

* 🐍 **Snake Mechanics**

  * Players move down when they land on a snake.
  * Snake positions are defined using JavaScript objects.

* 🪜 **Ladder Mechanics**

  * Players automatically climb when they land on a ladder.
  * Ladder start and destination positions are configurable.

* 👥 **Two-Player Gameplay**

  * Supports Player 1 and Player 2.
  * Each player has a separate position on the board.
  * Player turns automatically switch after each move.

* 🏆 **Winning System**

  * A player wins after reaching position 100.
  * The game stops accepting additional dice rolls after a winner is determined.
  * Players must roll the exact number required to reach 100.

* 🔄 **Restart Functionality**

  * The Restart button resets both players to the starting position.
  * The game state, dice display, messages, and turn order are reset.

* 📱 **Responsive Design**

  * The board adapts to different screen sizes.
  * CSS media queries improve usability on smaller devices.
  * Flexible font sizes and dimensions help maintain the layout across desktop and mobile screens.

## 🧠 How the Game Works

The game uses JavaScript objects to store the locations of snakes and ladders. For example, landing on a snake position moves the player to a lower position, while landing on a ladder position moves the player forward.

Each player is represented by an object containing their current position and CSS class. The application keeps track of whose turn it is using the `currentPlayer` variable.

When the **Roll Dice** button is clicked:

1. A random number between 1 and 6 is generated.
2. The current player's position is increased by that number.
3. The application checks whether the new position contains a ladder or snake.
4. The player's position is updated accordingly.
5. The board visually displays the player's new position.
6. The application checks whether the player has reached position 100.
7. If the player has not won, the turn changes to the other player.

The game also prevents players from moving beyond position 100 and requires an exact roll to finish the game.

## 🎨 User Interface

The interface contains:

* Game title
* 10×10 game board
* Numbered cells from 1–100
* Visual identification of snake and ladder cells
* Player tokens
* Dice display
* Current-turn/game-status message
* Roll Dice button
* Restart button
* Player legend

The board is generated dynamically through JavaScript instead of manually writing all 100 cells in HTML. The code also alternates the direction of each row to reproduce the traditional Snake & Ladder board layout.

## 🛠️ Technologies Used

### HTML5

Used to create the basic structure of the game, including the game container, board, controls, buttons, dice display, and status messages.

### CSS3

Used for:

* Responsive layout
* Game board styling
* Player tokens
* Snake and ladder colors
* Buttons and hover effects
* Mobile responsiveness
* Typography and visual design

The game uses a responsive 10-column CSS Grid for the board and includes a mobile media query for smaller screens.

### JavaScript

JavaScript handles the complete game logic, including:

* Board generation
* Player movement
* Dice generation
* Snake and ladder logic
* Turn switching
* Winner detection
* Game reset
* DOM manipulation
* Button event handling

The Roll Dice and Restart buttons are connected to their respective JavaScript functions using event listeners.

## 📂 Project Structure

```text
snake-and-ladder/
│
└── index.html
```

The current version is implemented as a **single HTML file**, containing the HTML structure, CSS styling, and JavaScript game logic.

## ▶️ How to Run

1. Download or clone the repository.
2. Open the project folder.
3. Open `index.html` in any modern web browser.
4. Click **Roll Dice** to start playing.
5. Use **Restart** to begin a new game.

No backend server, database, or external installation is required.

## 📚 What This Project Demonstrates

This project is useful for demonstrating practical frontend development concepts such as:

* DOM manipulation
* JavaScript variables and objects
* Arrays and conditional logic
* Functions
* Random number generation
* Event listeners
* Dynamic HTML generation
* CSS Grid
* Responsive web design
* Game-state management
* User interaction handling

## 🔮 Possible Future Improvements

The project can be extended with:

* Single-player mode against an AI
* 3–4 player support
* Dice rolling animation
* Player movement animation
* Sound effects
* Custom board themes
* Score/history tracking
* Difficulty levels
* Online multiplayer
* Local storage for saved games
* Improved accessibility features

## 👨‍💻 Project Purpose

This project was developed as a **frontend JavaScript game project** to demonstrate the implementation of interactive game logic and responsive user interfaces using standard web technologies.

It provides a simple example of how **HTML, CSS, and JavaScript can work together to create a complete playable browser game without requiring a backend**.
