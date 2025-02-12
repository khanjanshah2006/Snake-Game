# Snake Game (C++)

## TEAM NULL POINTERS

- [KHANJAN SHAH](https://github.com/khanjanshah2006)
- [NISHITH THATHAGAR](https://github.com/Nishith1130)
- [KARTIK SHAH](https://github.com/Kartik21407)
- [RAHUL KARIYA](https://github.com/RahulKariya049)

## 🌟 Table of Contents
- Project Description
- Key Features
- Installation
- Gameplay Controls
- How To Play
- Data Structure Analysis
- Object Oriented Structure
- Key Member Functions
- Difficulty Levels
- Code Structure
- Prerequisites
- License

## Project Description

This project implements the classic *Snake Game* using C++ with a linked list-based approach. It showcases essential Object-Oriented Programming (OOP) concepts.

Players control a snake on a 2D grid, eating food (F) that appears randomly while avoiding collisions with the walls and the snake's body.

## Key Features

1. *Interactive Gameplay:* Control the snake using keyboard keys (W, A, S, D).
2. *Dynamic Snake Growth:* Eating food increases the snake's length.
3. *Random Food Generation:* Food appears at random positions avoiding collision with the snake.
4. *Game Over Conditions:* The game ends if the snake collides with itself or the walls.
5. *Difficulty Levels:* Choose between Easy, Medium, or Hard mode.
6. *High Score Tracking:* Separate high scores for each difficulty level.

## Installation

To run the Snake game, follow these steps:
1.  **Clone the Repository:**
    ```bash
    $ git clone [https://github.com/yourusername/snake-game-cpp.git](https://github.com/yourusername/snake-game-cpp.git)
    $ cd snake-game-cpp
    ```
2.  **Compile the Code (using g++):**
    ```bash
    $ g++ snake_game.cpp -o snake_game.exe
    ```
3.  **Run the Game:**
    ```bash
    $ ./snake_game.exe
    ```
---

## Gameplay Controls

- W : Move Up  
- A : Move Left  
- S : Move Down  
- D : Move Right  
- X : Exit the Game  
- P : Play Again  
- M : Return to Menu  
---

## How To Play

1. *Select Difficulty Level:*
   - Press 'A' for Easy (200ms delay)
   - Press 'B' for Medium (120ms delay)
   - Press 'C' for Hard (80ms delay)
3. *Objective:* Eat food (F) to grow and avoid hitting walls or yourself.
4. *Game Over:* If the snake crashes into itself or the boundaries.
5. *Restart:* Press P to restart, M to go back to menu, or X to exit.

---
## Data Structure Analysis

- Linked List → Used for the snake’s body (each segment as a Node).
- Enums → Direction for movement, Difficulty for game speed.
- Classes:
    - Snake → Handles movement & collisions.
    - Food → Generates food at random positions.
    - GameLogic → Manages game flow & rendering.
- High Scores → Stored per difficulty level & updated after each game.

---

## Object-Oriented Structure

| Class           | Responsibility                                                   |
|----------------|-----------------------------------------------------------------|
| Snake| Manages the snake's movement, direction, and collision detection |
| Food | Handles spawning and position tracking of food item|
| GameLogic | Controls the game loop, input handling, rendering and scoring|

## Key Member Functions

### Snake Class
- `changeDirection(Direction dr)` → Updates snake’s movement direction.
- `move()` → Moves snake in the current direction.
- `RemoveLastSegment()` → Removes the last tail segment.
- `collideWithSelf()` → Checks if the snake collides with itself.
- `collidesWithWall()` → Detects wall collision.

### Food Class
- `spawn(Snake &snake)` → Generates food at a random position.

### GameLogic Class
- `draw()` → Renders the game board.
- `input()` → Handles user input for movement.
- `update()` → Updates game state (movement, collision, score).
- `isGameOver()` → Checks if the game is over.
- `delay(int ms)` → Controls game speed based on difficulty.

---
## Difficulty Levels

- **Easy** → 200ms delay (Slower, relaxed gameplay).
- **Medium** → 120ms delay (Balanced speed).
- **Hard** → 80ms delay (Fast, challenging mode).

---
## 📁 Code Structure
📂 Snake Game/  
│── 📄 README.md  
│── 📄 snake_game.cpp  
│── 📄 LICENSE

## Prerequisites
- A C++ compiler (e.g g++)
- Windows (modifications required for Linux)

## 🌟 License

This project is open-source and available under the MIT License. Feel free to modify and use it for educational purposes! 🎉


🎉 Thanks for checking out this project! Hope you enjoy playing! 🚀
