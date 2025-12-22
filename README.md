# Drone Defender

A 2D arcade-style shooter built with Python and Pygame. Pilot your ship, avoid waves of drones, and survive by blasting enemies while dodging incoming projectiles. The game features animated sprites, enemy AI, collision mechanics, scoring, and asset-based visuals and sound.

---

## Features

* Player-controlled ship with smooth movement and shooting
* Autonomous drones with randomized attack patterns
* Downward-firing enemy projectiles
* Collision detection between bullets, drones, and the player
* Scoring and progression logic
* Asset-driven art and sound (images, icons, etc.)
* Modular, multi-file Python codebase for easier maintenance and extension
* Packaged and build-ready with PyInstaller

---

## Requirements

* Python 3.8 or later
* Pygame
* Pygame-widgets
* sys
* random
* utils

Example installation:

```bash
pip install pygame pygame-widgets
```

---

## How to Play

* Move using the arrow keys or WASD
* Fire bullets with your defined shoot key (typically Spacebar)
* Destroy drones before they reach or hit you
* Avoid incoming enemy bullets
* Survive as long as possible and maximize your score

---

## Project Structure Overview

```
project/
│
├── main.py                # Entry point and game loop
├── player.py              # Player logic and controls
├── drone.py               # Enemy behavior and movement
├── bullet.py              # Projectile classes
├── assets/
│   ├── images/            # Sprites and background art
│   ├── sounds/            # Sound effects and music
│   └── icons/             # Game window + exe icon
└── README.md
```


---

## Packaging as an Executable

This game can be bundled as a `.exe` using PyInstaller. A typical build command:

```bash
pyinstaller --onefile --add-data '*.png:.' --icon=icon.ico main.py
```

This ensures all dependent images and sounds are included and the icon is applied.

---

## Known Issues / Future Enhancements

* Balancing enemy bullet speed and spawn intervals
* Expanded level progression
* Improved UI/menus
* Enhanced particle effects and animations
* High-score persistence

---
