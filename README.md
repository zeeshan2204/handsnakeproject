🐍 HandSnakeProject

Gesture-Controlled Nokia Snake Game using OpenCV, MediaPipe & Pygame

Control the classic Nokia Snake game with your hand gestures using your webcam.
Move your hand to steer the snake and use a pinch gesture for speed boost.

This project combines computer vision, real-time gesture recognition, and a retro snake game into one interactive experience.

🎮 Features

✋ Hand gesture control (Up, Down, Left, Right)

🤏 Pinch gesture = Speed boost

🎥 Real-time webcam tracking with MediaPipe

🐍 Classic Nokia-style snake gameplay

💥 Particle effects when eating fruit

🔁 Gesture-based restart (show UP after game over)

🧵 Multithreaded gesture detection for smooth gameplay

🟩 Retro green Nokia theme UI

🧠 How It Works

MediaPipe Hands detects your hand landmarks from the webcam

Wrist movement → Direction control

Thumb + Index finger close → Speed boost

Pygame runs the snake game while OpenCV handles gesture tracking in a separate thread 

Gesture detection logic is implemented in the GestureController class using wrist movement vectors and pinch distance thresholds 

.

🕹️ Controls
Gesture	Action
Move hand up/down/left/right	Control snake direction
Pinch (thumb + index)	Speed boost
Show UP after Game Over	Restart game
Press ESC	Quit game
📁 Project Structure
HandSnakeProject/
│── main.py                 # Game manager & threading
│── snake_game.py           # Nokia-style snake implementation
│── gesture_controller.py   # Hand tracking & gesture logic
│── requirements.txt        # Python dependencies
│── setup.py                # Auto installer script

⚙️ Requirements

Python 3.9+ recommended

Dependencies:

opencv-python

mediapipe

numpy

pygame 

🚀 Installation
1️⃣ Clone the repository
git clone https://github.com/zeeshan2204/HandSnakeProject.git
cd HandSnakeProject

2️⃣ Install dependencies

Option A — Automatic setup:

python setup.py


Option B — Manual:

pip install -r requirements.txt

▶️ Run the Game
python main.py


Make sure your webcam is connected and accessible.

Two windows will open:

🎮 Snake Game Window (Pygame)

🎥 Gesture Control Window (Webcam feed)

🧩 Technical Details
Gesture Detection

Uses MediaPipe Hands

Tracks wrist position for swipe direction

Uses Euclidean distance between thumb tip and index tip for pinch detection

Includes gesture cooldown to prevent rapid direction flipping 

Game Engine

Built with Pygame

Grid-based movement

Direction reversal protection

Particle effects on fruit consumption

Dynamic speed based on pinch gesture 

Performance

Gesture detection runs in a separate thread

Game loop maintains consistent FPS

Camera processed at ~30 FPS 

🖥️ System Requirements

Webcam

Python 3.9+

Works on Windows, Linux, macOS (with webcam support)

🧪 Troubleshooting

Webcam not detected

Close other apps using the camera

Check camera permissions

Low FPS / Lag

Ensure good lighting

Keep hand within camera frame

Reduce background processes

Gestures not detected

Show one hand only

Keep wrist visible

Move hand clearly in one direction

🌟 Future Improvements

Gesture sensitivity calibration

Hand tracking for both hands

On-screen gesture guide

Score leaderboard

Mobile / web version

AI difficulty scaling

📜 License

MIT License

🙌 Acknowledgements

MediaPipe for real-time hand tracking

OpenCV for video processing

Pygame for game rendering

💡 Demo Idea

Record a short GIF showing:

Hand moving → snake turning

Pinch → speed boost

Game over → UP gesture → restart

