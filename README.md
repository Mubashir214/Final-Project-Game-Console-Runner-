# Final-Project-Game-Console-Runner-.

📘 README.md
Final Project Game – Console Runner

Author: Mubashir
Language: C++
Platform: Windows Console
File: main.cpp

🎮 Game Overview

This is a simple endless runner console game developed as a final-term project.
Your objective is to survive as long as possible by avoiding obstacles (X) and collecting coins (o).
The longer you stay alive, the more miles you cover, and coins increase your score.

The game runs inside a 15×18 character grid, with smooth movement, jump/slide actions, score tracking, and automatic obstacle generation.

✨ Features
👾 Player Actions

Move Up: W

Move Down: S

Move Left: A

Move Right: D

Jump: J

Slide: K

Quit Game: Q

💥 Game Mechanics

Obstacles (X) fall from the top.

Coins (o) spawn randomly.

Jumping or sliding can help avoid some hits.

Collision with an obstacle reduces life.

Collecting coins increases score.

Every refresh increases miles.

📊 Scoring System

Lives: 3 total

Miles: Increase automatically as you survive

Coins: +1 per coin collected

All results are saved to data.txt in the format:

Name Miles Score

🧱 Game World

Grid Size: 18 rows × 15 columns

Special Characters:

Character	Meaning
@	Player
^	Jumping Player
`	Sliding Player
X	Obstacle
o	Coin
📂 File Output

All game results (Player Name, Miles, Score) are stored in:

data.txt


This allows tracking multiple play sessions.

▶️ How to Run

Compile using any C++ compiler (MinGW, Dev-C++, Code::Blocks, Visual Studio).

Make sure conio.h and windows.h are available (Windows OS required).

Run the executable.

Example command:

g++ main.cpp -o game.exe
game.exe

📸 Screenshot (console preview)
|             |
|      o      |
|             |
|      X      |
|             |
|     @       |
---------------
Miles: 24m
Lifes: 3
Coins: 2

📜 Code Summary

The game uses:

Real-time keyboard detection (_kbhit(), _getch()).

Frame-based action timing (jump & slide duration).

Auto-scrolling grid updates.

Randomized obstacle & coin spawning.

Game state saving using file handling.
