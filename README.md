# 🟡 PACMAN Game – OOP C++ Project

**PACMAN Game** is a C++ console-based recreation of the classic arcade game, developed as a course project for Object-Oriented Programming (OOP). Players control Pacman to collect dots in a maze while avoiding enemy ghosts. The game includes multiple difficulty levels, colorful visuals, sound effects, and a persistent scoreboard system.

---

## 📋 Table of Contents

- [🎮 Features](#-features)
- [🕹️ How to Play](#-how-to-play)
- [⚙️ Technical Details](#-technical-details)
- [📦 Requirements](#-requirements)
- [🚀 Installation](#-installation)
- [📘 Usage](#-usage)
- [💡 Notes](#-notes)
- [👨‍💻 Credits](#-credits)

---

## 🎮 Features

### 🎯 Difficulty Levels
- **Easy** – 121 dots
- **Medium** – 172 dots
- **Hard** – 358 dots

### 🧠 Gameplay Mechanics
- Arrow key movement
- Dot collection increases score
- Ghosts use **Breadth-First Search (BFS)** for chasing
- Win by collecting all dots, lose if caught by a ghost

### 🎧 Audio
- Selectable background music (e.g., WWE themes like *Worlds Apart*, *Cult of Personality*)
- Sound effects for victory and defeat

### 📊 Score & Records
- Tracks player score based on collected dots
- Records player name, score, and difficulty level in `PacmanGameRecordsList.txt`

### 🎨 Visuals
- Uses Windows console text colors:
  - Pacman: **Yellow**
  - Ghosts: **Red**, **Pink**, **Purple**
  - Walls: **Blue/Cyan**
  - Dots: **Green**

---

## 🕹️ How to Play

1. **Launch the Game**  
   Run the `.exe` file to start the intro screen with credits and music.

2. **Main Menu Options**
   - `P` – Play Game
   - `M` – Change Background Music
   - `D` – View Player Records
   - `E` – Exit

3. **Game Flow**
   - Enter your name
   - Select difficulty level (1-3)
   - Use arrow keys to move and collect dots
   - Win: Collect all dots  
   - Lose: Get caught by a ghost

4. **Post-game**
   - Your score and data are saved in `PacmanGameRecordsList.txt`

---

## ⚙️ Technical Details

- **Language:** C++
- **Platform:** Windows Console
- **Libraries Used:**
  - Standard: `iostream`, `vector`, `string`, `fstream`
  - Windows-specific: `windows.h`, `conio.h`, `mmsystem.h` (`PlaySound`)

### 🔧 Object-Oriented Structure

| Class         | Responsibility                                 |
|---------------|------------------------------------------------|
| `map`         | Maze design and layouts for each level         |
| `entity`      | Base class for characters (Pacman and Ghosts)  |
| `Pacman`      | Player character and movement logic            |
| `Enemy`       | Ghost logic and BFS pathfinding                |
| `Player`      | Controls game state and character interaction  |
| `ScoreBoard`  | Tracks and displays score                      |
| `Audio`       | Manages background music                       |
| `losewinSound`| Plays victory/defeat sound effects             |
| `PlayersData` | Handles saving and displaying records          |
| `Game`        | Game flow, menus, and intro logic              |

---

## 📦 Requirements

- Windows OS (console-specific)
- Sound files (e.g., `8-Bit-Cody-Rhodes.wav`, `mixkit-video-game-win-2016.wav`) in the same directory as the `.exe`
- C++ compiler with Windows API support:
  - MinGW (TDM-GCC)
  - MSVC (Visual Studio)

---

## 🚀 Installation

1. **Clone the repo**
   ```bash
   git clone https://github.com/yourusername/OOP_PACMAN_GAME.git
   cd OOP_PACMAN_GAME
   ```

2. **Ensure sound files** are in the same directory as the `.exe`

3. **Build the project**
   ```bash
   mingw32-make
   ```

4. **Run the game**
   ```bash
   ./PACMAN-SABIH_ANAS_ARHAMOOP.exe
   ```

---

## 📘 Usage

- Run the game and follow the menu prompts.
- Play the game with arrow keys.
- View player records from the main menu.

---

## 💡 Notes

- This game is designed for **Windows consoles only** and may not run on other platforms without modification.
- Sound features will not work if the `.wav` files are missing.
- Ghost movement via BFS may be predictable; adding randomness would enhance difficulty.

---

## 👨‍💻 Credits

Developed by:

- **Sabih Uddin** (k224347@nu.edu.pk)  
- **Anas Khan** (anacekhanx@gmail.com)  
- **Arham Khan** (k224542@nu.edu.pk)  

As a final project for the **Object-Oriented Programming** course.

---
