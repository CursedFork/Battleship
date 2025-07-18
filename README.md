# Battleship AI Web App

A modern web-based version of the classic board game *Battleship*, featuring multiple AI opponents with unique attack strategies. This project aims to demonstrate a variety of search and decision-making algorithms through a fun and interactive interface.

---

## Basic Rules of Battleship

Battleship is a two-player guessing game where each player places ships on a grid and then takes turns attacking the opponent’s grid.

- Each player places 5 ships of varying lengths on a 10x10 grid.
- The ships cannot overlap and must be placed horizontally or vertically.
- Players take turns entering coordinates (e.g., B5) to "attack."
- The opponent must respond with “hit” or “miss.”
- When all the cells of a ship are hit, it is “sunk.”
- The first player to sink all opposing ships wins.

---

## AI Opponent Strategies (Planning - Not Final at Present)

This app includes several AI opponents, each designed to demonstrate different algorithms and strategies:

### 1. **Random Shooter**
- Attacks random coordinates without tracking previous moves.
- Simple, unpredictable, and baseline for comparison.

### 2. **Smart Random with Minimax Targeting**
- Starts with random attacks.
- When it hits a ship, it switches to a localized minimax pattern to destroy it efficiently.

### 3. **Checkerboard Search**
- Since the smallest ship is 2 units long, hitting every other square should guarantee that no ship could be missed
- This reduces the number of necessary guesses significantly compared to random shooting

### 3. **Probability Heatmap AI (Optional Advanced)**
- Uses probability maps to find the most likely ship placements.
- Dynamically updates based on hits and misses.

Each AI will have its own module with documented logic, performance metrics, and a difficulty rating.

---

## Technologies Used 

- **React.js** – For UI and component management.

---

## Planned Features

- Save/load games
- Player vs Player mode
- Scoreboard with AI win rates
