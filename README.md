# Simon Says Game

A web-based memory sequence game that challenges players to track and repeat an ever-growing pattern of colors and flashes.
## 🎮 How to Play

* **Start the Game**: Press any key on your keyboard to initiate the first level.
* **Watch the Pattern**: The game will randomly select a button and "flash" it white to show the sequence.
* **Repeat the Sequence**: Click the buttons in the exact order they were presented.
* **Level Up**: Successfully completing the sequence moves you to the next level, adding one more color to the pattern.
* **Game Over**: If you click the wrong button, the background flashes red, and your final score is displayed.

## 🚀 Features
* **Dynamic Leveling**: The game tracks your progress and increases difficulty indefinitely as you succeed.
* **Visual Feedback**:
* **Game Flash**: Buttons flash white (`whitesmoke`) when the system is demonstrating the sequence.
* **User Flash**: Buttons flash green when clicked by the player.
* **Failure Alert**: The background turns red briefly to signal a wrong move.
* **Score Tracking**: The `h2` header updates in real-time to show your current level and your final score upon losing.

## 🛠️ Technologies Used
* **HTML5**: Provides the game structure, including the button container and level headers.
* **CSS3**: Handles the 2x2 grid layout, button styling (rounded corners, specific colors), and flash effects.
* **JavaScript (Vanilla)**: Manages the game logic, random color generation, sequence validation, and event listeners for both keypresses and clicks.

## 📂 Project Structure
* `index.html`: Contains the four game buttons (Red, Light-Blue, Yellow, Gray) and the game interface.
* `style.css`: Defines the visual appearance, including the flexbox container and button classes.
* `app.js`: Contains the core logic, including `levelUp()`, `checkAns()`, and the sequence arrays.

## ⚙️ Logic Summary
* **Sequence Storage**: The game uses `gameseq` to store the generated pattern and `userseq` to track player inputs.
* **Randomization**: A random index is used to pick one of the four colors from the `btns` array: `["red", "light-blue", "yellow", "gray"]`.
* **Reset Mechanism**: Upon losing, the `reset()` function clears the level and sequences so the player can start fresh.

⚙️ Setup & Installation
To run this game locally on your machine, follow these steps:
Clone the Repository:
git clone https://github.com/your-username/simon-says-game.git
Navigate to the Directory:
cd simon-says-game
Launch the Game:
Simply locate the index.html file in your file explorer and double-click it to open it in your default web browser.
Alternatively, if you use VS Code, right-click index.html and select "Open with Live Server".
