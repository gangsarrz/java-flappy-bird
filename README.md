# 🐦 Java Flappy Bird

> A simple Flappy Bird clone built using Java and Java Swing.
> This project was created to practice Object-Oriented Programming (OOP), Java GUI development, game loops, collision detection, and event handling.

---

## 📸 Preview

> Add screenshots or GIF here

| Main Menu | Gameplay |
|-----------|-----------|
| ![](images/menu.png) | ![](images/gameplay.png) |

Or

![Gameplay Demo](images/demo.gif)

---

# 📖 Table of Contents

- Overview
- Features
- Technologies Used
- Project Structure
- How It Works
- Installation
- Running the Project
- Controls
- Game Mechanics
- OOP Concepts Used
- Future Improvements
- Learning Outcomes
- Known Issues
- Contributing
- License
- Author

---

# 📌 Overview

Java Flappy Bird is a desktop game inspired by the classic Flappy Bird.

The objective is simple:

- Control the bird
- Avoid hitting pipes
- Try to achieve the highest score possible

This project focuses on implementing game development fundamentals using pure Java without external game engines.

---

# ✨ Features

- Bird movement with gravity
- Jump mechanics
- Random pipe generation
- Collision detection
- Score system
- Game Over screen
- Restart game
- Smooth animation using game loop
- Keyboard controls
- Simple pixel-style gameplay

---

# 🛠 Technologies Used

- Java
- Java Swing
- Java AWT
- OOP (Object-Oriented Programming)

No external libraries are required.

---

# 📂 Project Structure

Example:

```
java-flappy-bird
│
├── src
│   ├── Main.java
│   ├── GamePanel.java
│   ├── Bird.java
│   ├── Pipe.java
│   ├── Game.java
│   └── assets
│       ├── bird.png
│       ├── pipe.png
│       └── background.png
│
├── images
│
├── README.md
│
└── LICENSE
```

> Your structure may be different depending on your project.

---

# ⚙ How It Works

The game continuously performs these steps:

```
Start Game

↓

Initialize Bird

↓

Generate Pipes

↓

Game Loop

↓

Update Bird Position

↓

Move Pipes

↓

Check Collision

↓

Increase Score

↓

Render Graphics

↓

Repeat Until Game Over
```

The game loop is responsible for:

- Updating object positions
- Detecting collisions
- Redrawing the screen
- Maintaining FPS

---

# 🚀 Installation

## 1 Clone Repository

```bash
git clone https://github.com/gangsarrz/java-flappy-bird.git
```

---

## 2 Open Project

Open using

- IntelliJ IDEA
- Eclipse
- NetBeans
- VS Code (Java Extension Pack)

---

## 3 Compile

```bash
javac *.java
```

or using your IDE.

---

# ▶ Running the Project

Run:

```bash
java Main
```

or simply click **Run** inside your IDE.

---

# 🎮 Controls

| Key | Action |
|------|----------|
| Space | Jump |
| R | Restart Game *(optional)* |
| ESC | Exit *(optional)* |

---

# 🎯 Game Mechanics

## Gravity

The bird constantly falls due to gravity.

```
velocity += gravity
position += velocity
```

---

## Jump

When the player presses **Space**:

```
velocity = jumpForce
```

The bird moves upward.

---

## Pipe Generation

Pipes are generated at random heights with a fixed gap between the top and bottom pipes.

Example:

```
Pipe

█████

Gap

█████
```

---

## Collision Detection

The game checks collision between:

- Bird vs Top Pipe
- Bird vs Bottom Pipe
- Bird vs Ground
- Bird vs Ceiling

If a collision occurs:

```
Game Over
```

---

## Score System

The score increases every time the bird successfully passes a pipe.

Example:

```
Bird

↓

Pipe

✔ Score +1
```

---

# 🧠 Object-Oriented Programming Concepts

This project demonstrates several OOP principles.

## Encapsulation

Each game object manages its own data.

Example:

- Bird
- Pipe

---

## Abstraction

Game logic is separated into different classes.

---

## Inheritance *(if implemented)*

Can be extended for future entities.

---

## Polymorphism *(optional)*

Useful when adding enemies or collectibles.

---

# 📚 Learning Outcomes

Through this project, I learned about:

- Java Swing
- Java Graphics
- Event Handling
- Keyboard Listener
- Timers
- Animation
- Collision Detection
- Random Generation
- Object-Oriented Programming
- Game Development Basics
- Code Organization
- Debugging Java Applications

---

# 📈 Future Improvements

Planned features:

- Sound effects
- Background music
- High score saving
- Difficulty levels
- Pause menu
- Animated bird
- Better graphics
- Mobile version
- Power-ups
- Multiple bird skins

---

# 🐞 Known Issues

- Window resizing is not supported.
- Score resets after restarting.
- No save/load system.
- Basic collision detection.

---

# 🤝 Contributing

Contributions are welcome.

If you'd like to improve this project:

1. Fork the repository

2. Create a new branch

```bash
git checkout -b feature/new-feature
```

3. Commit changes

```bash
git commit -m "Add new feature"
```

4. Push

```bash
git push origin feature/new-feature
```

5. Open a Pull Request

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub.

It motivates me to build more open-source projects and continue learning.