🐍 HandSnakeProject

Gesture-Controlled Nokia Snake Game using OpenCV, MediaPipe & Pygame

Play the classic Nokia Snake game using hand gestures through your webcam.
Move your hand to control the snake and pinch your fingers to activate speed boost.

This project combines computer vision, real-time gesture recognition, and retro game development in Python.

🎮 Features

✋ Control snake using hand movement (Up, Down, Left, Right)

🤏 Pinch gesture for speed boost

🐍 Classic Nokia-style snake gameplay

💥 Particle effects when eating fruit

🔁 Gesture-based restart after game over

🧵 Multithreaded gesture detection for smooth performance

🎥 Live webcam feed with hand tracking overlay

🟩 Retro green Nokia theme UI

🧠 How It Works

MediaPipe Hands detects hand landmarks from the webcam

Wrist movement determines snake direction

Thumb + Index finger distance detects pinch → activates speed boost

Gesture detection runs in a separate thread while the game runs in Pygame for smooth gameplay 

main

🕹️ Controls
Gesture	Action
Move hand up/down/left/right	Control snake direction
Pinch (thumb + index finger)	Speed boost
Show UP after game over	Restart game
Press ESC	Quit game
📁 Project Structure
HandSnakeProject/
│── main.py                 # Game manager & threading
│── snake_game.py           # Nokia-style snake implementation
│── gesture_controller.py   # Hand tracking & gesture logic
│── requirements.txt        # Dependencies
│── setup.py                # Auto installer script

⚙️ Requirements

Python 3.9+

Webcam

Python libraries:

opencv-python

mediapipe

numpy

pygame 

requirements

🚀 Installation
1️⃣ Clone the repository
git clone https://github.com/yourusername/HandSnakeProject.git
cd HandSnakeProject

2️⃣ Install dependencies
Option A — Automatic setup
python setup.py

Option B — Manual
pip install -r requirements.txt

▶️ Run the Game
python main.py


Two windows will open:

🎮 Snake Game Window

🎥 Gesture Control Window

Make sure your webcam is connected and accessible.

🧩 Technical Details
Gesture Detection

Uses MediaPipe hand landmarks

Wrist movement → direction detection

Pinch detection using Euclidean distance between thumb and index finger

Gesture cooldown prevents rapid direction flipping 

gesture_controller

Game Engine

Built with Pygame

Grid-based movement

Direction reversal protection

Particle effects on fruit consumption

Dynamic speed (normal vs boost) 

snake_game

Performance

Gesture detection runs at ~30 FPS in a separate thread

Game loop maintains stable rendering and input handling 

main

🖥️ System Requirements

Webcam

Python 3.9+

Works on Windows, Linux, and macOS (with webcam support)

🧪 Troubleshooting

Webcam not detected

Close other apps using the camera

Check camera permissions

Gestures not working

Use good lighting

Keep one hand in frame

Move hand clearly in one direction

Keep wrist visible to the camera

Low FPS

Reduce background apps

Ensure adequate lighting for faster hand tracking

🌟 Future Improvements

Gesture sensitivity calibration

On-screen gesture guide

Dual-hand support

Score leaderboard

AI difficulty scaling

Web/mobile version

📜 License

MIT License

🙌 Acknowledgements

MediaPipe – Hand tracking

OpenCV – Video processing

Pygame – Game rendering

💡 Demo Tip

Hand movement → snake turns

Pinch → speed boost

Game over → UP gesture → restart

This will make your repo stand out to recruiters.
