Car Game Using Python  
A 2D endless-style car game built with Python and Pygame. Drive through a three-lane road, avoid oncoming traffic, and try to achieve the highest score as the game gradually gets faster.
Features
- Three-lane road with animated lane markings.
- Player-controlled car with left and right lane movement.
- Randomly generated traffic using different vehicle sprites.
- Collision detection for head-on collisions and side swipes.
- Score increases whenever an oncoming vehicle passes the screen.
- Game speed increases after every five vehicles passed.
- Background music and a crash sound effect.
- Restart option after a game-over event.
Tech Stack
- Language: Python 3
- Library: Pygame
- Modules: random, os, and Pygame modules for graphics, sprites, keyboard input, and audio
Project Structure
Keep the image and sound assets in the folders shown below. The filenames must match the paths used by main.py.
car-game-using-python/
├── main.py
├── requirements.txt
├── images/
│   ├── car.png
│   ├── pickup_truck.png
│   ├── semi_trailer.png
│   ├── taxi.png
│   ├── van.png
│   └── crash.png
└── sounds/
    ├── background_music.mp3
    └── crash_sound.wav
Prerequisites
- Python 3.x
- A desktop environment capable of opening a Pygame window
- The image and audio assets listed in the project structure
Installation
1. Clone this repository:
   git clone https://github.com/Iris3014/car-game-using-python.git
   cd car-game-using-python
2. (Recommended) Create and activate a virtual environment:
   Windows
   python -m venv .venv
   .venv\Scripts\activate
   macOS / Linux
   python3 -m venv .venv
   source .venv/bin/activate
3. Install Pygame:
   python -m pip install -r requirements.txt
Run the Game
Run the following command from the project directory:
python main.py
Controls
Key	Action
← Left Arrow	Move the car one lane to the left
→ Right Arrow	Move the car one lane to the right
Y	Restart after Game Over
N	Exit after Game Over


You can also close the game window to quit.
Gameplay
1. The player's car starts in the center lane.
2. Use the arrow keys to move between the three lanes.
3. Avoid colliding with incoming vehicles.
4. Earn one point each time a vehicle passes off the bottom of the screen.
5. The game gets faster after every five vehicles passed.
6. If a collision occurs, choose Y to play again or N to exit.
Troubleshooting
- Missing image error: Check that the images directory exists and contains every required image with the exact filename and capitalization.
- Missing sound error: Check the sounds directory and confirm that both audio files are present.
- No audio: Check your system's audio output. The game initializes Pygame's mixer, so an audio-device or mixer initialization issue may prevent startup.
- Pygame not found: Activate your virtual environment and run python -m pip install -r requirements.txt.
- Game window does not open: Run the command from a local desktop session with graphics support rather than a headless terminal.
Implementation Notes
- The game window is 500 × 500 pixels and targets 120 frames per second.
- The road has three lanes, and traffic vehicles are selected randomly from the available vehicle images.
- Image and audio assets are loaded using relative paths, so run main.py from the repository's root directory.
- The game uses Pygame sprite groups for the player and traffic vehicles.
Possible Enhancements
- Add a pause/resume feature.
- Add a high-score table that persists between runs.
- Add difficulty settings and more traffic patterns.
- Improve responsive layout and add a start screen.
- Handle unavailable audio devices and missing assets more gracefully.
