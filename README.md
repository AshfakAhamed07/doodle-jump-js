# Doodle Jump

A simple browser-based Doodle Jump-inspired game built with **HTML, CSS, and vanilla JavaScript**.

This project was created as a hands-on JavaScript learning project by following a Doodle Jump game development tutorial and implementing the concepts step by step. The goal was to strengthen understanding of JavaScript game logic, DOM manipulation, timers, event handling, collision detection, and basic game mechanics.

## 🎮 Features

* Player character (Doodler) with automatic jumping
* Gravity and falling mechanics
* Randomly generated platforms
* Platform collision detection
* Automatic platform scrolling
* Horizontal player movement
* Left and right wall bouncing
* Score tracking
* Game-over state
* Dynamic creation and removal of game elements

## 🛠️ Technologies

* **HTML5** — Game structure
* **CSS3** — Game layout and styling
* **JavaScript (ES6+)** — Game logic and interactions
* **DOM API** — Dynamic game element creation and manipulation
* **Git & GitHub** — Version control and project management

## 🎯 Controls

| Key | Action                   |
| --- | ------------------------ |
| `←` | Move left                |
| `→` | Move right               |
| `↑` | Stop horizontal movement |

The Doodler automatically jumps when landing on platforms.

## 📁 Project Structure

```text
doodle-jump-js/
├── index.html
├── style.css
├── script.js
└── README.md
```

## 🧠 What I Learned

This project helped me practice several important JavaScript concepts:

* `DOMContentLoaded`
* DOM element creation with `createElement()`
* `querySelector()`
* `appendChild()`
* CSS manipulation through JavaScript
* JavaScript classes
* Arrays and objects
* `setInterval()` and `clearInterval()`
* Keyboard event handling
* Collision detection
* Random number generation
* Game state management
* Basic game loops
* Managing multiple timers
* Dynamic creation and removal of DOM elements

## ⚙️ How the Game Works

### 1. Creating the Doodler

The player character is created dynamically using JavaScript and positioned inside the game grid.

```js
const doodler = document.createElement("div");
doodler.classList.add("doodler");
```

### 2. Generating Platforms

Platforms are represented using a JavaScript `Platform` class. Their horizontal positions are randomly generated so that the game layout changes between runs.

```js
this.left = Math.random() * 315;
```

### 3. Jumping and Falling

The Doodler continuously jumps and falls using timed intervals.

The jumping process increases the player's vertical position, while the falling process decreases it.

### 4. Platform Collision

While falling, the game checks whether the Doodler's position overlaps with a platform.

When a collision occurs, the Doodler lands on the platform and begins another jump.

### 5. Scrolling Platforms

As the Doodler climbs higher, platforms move downward.

Platforms that leave the game area are removed and replaced with new platforms at the top.

### 6. Player Movement

The arrow keys control horizontal movement.

The Doodler can move left and right and will bounce back when reaching the boundaries of the game area.

### 7. Scoring

The score increases as platforms are passed and recycled.

### 8. Game Over

When the Doodler falls below the game area, the game ends and the final score is displayed.

## 🚀 Running the Project

Clone the repository:

```bash
git clone https://github.com/AshfakAhamed07/doodle-jump-js.git
```

Open the project folder:

```bash
cd doodle-jump-js
```

Then open `index.html` in your browser.

You can also use **VS Code with Live Server** to run the project locally.

## 📌 Future Improvements

Possible improvements for future versions include:

* Add proper player and platform graphics
* Improve the visual design
* Add a start/restart button
* Add a high-score system
* Add sound effects and background music
* Add increasing difficulty
* Improve collision detection
* Add responsive controls
* Add mobile/touch support
* Improve the game-over screen
* Refactor the game loop and timer management

## 📚 Learning Purpose

This project is part of my ongoing JavaScript learning journey. It focuses on applying JavaScript concepts to a practical project rather than simply learning syntax in isolation.

The project also provides practice with Git and GitHub by developing the game incrementally and maintaining meaningful commits throughout the development process.

## 📄 License

This project is intended primarily for learning and educational purposes.
