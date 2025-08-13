# Car Game 🚗💨

A simple 2D car game built with Python and Pygame.  
The goal is to avoid oncoming vehicles, survive as long as possible, and increase your score as the game speeds up.

## Features
- **Three-lane road** with moving traffic.
- **Score system** – gain points by passing vehicles.
- **Speed increase** as you progress.
- **Collision detection** with crash animation.
- **Background music** and crash sound effects.
- **Replay option** after game over.

## Controls
- **Left Arrow (←)** – Move one lane left.
- **Right Arrow (→)** – Move one lane right.
- **Y** – Restart game after Game Over.
- **N** – Exit after Game Over.

## Requirements
- Python 3.x
- Pygame

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/car-game.git
    cd car-game
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Make sure you have the following folder structure:
    ```
    car-game/
    ├── main.py
    ├── images/
    │   ├── car.png
    │   ├── pickup_truck.png
    │   ├── semi_trailer.png
    │   ├── taxi.png
    │   ├── van.png
    │   └── crash.png
    ├── sounds/
    │   ├── background_music.mp3
    │   └── crash_sound.wav
    ├── requirements.txt
    └── README.md
    ```

4. Run the game:
    ```bash
    python car_game.py
    ```

## Notes
- Ensure the `images` and `sounds` folders contain all the required assets.
- Background music and sound effects may fail to load if the files are missing.

## License
This project is licensed under the MIT License.
