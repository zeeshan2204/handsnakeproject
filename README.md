# Gesture Controlled Snake Game  

A modern twist on the classic Nokia Snake game using real-time hand gesture recognition  

---

## Features

- 🎮 Control snake using hand gestures  
- ✋ Real-time hand tracking using MediaPipe  
- 🔥 Pinch gesture for speed boost  
- 🧠 AI-based gesture recognition  
- 🖥️ Classic Nokia-style snake UI  
- ⚡ Multi-threaded performance  

---

## 🛠 Tech Stack

| Category | Technology |
|----------|-----------|
| Language | Python |
| Computer Vision | OpenCV |
| Gesture Recognition | MediaPipe |
| Game Engine | Pygame |
| Data Processing | NumPy |

---

## 📂 Project Structure

```bash
Gesture-Snake-Game/
│── main.py                 # Main game controller
│── gesture_controller.py   # Gesture detection logic
│── snake_game.py           # Game implementation
│── setup.py                # Setup script
│── requirements.txt        # Dependencies
```

---

## 🚀 Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/yourusername/gesture-snake-game.git
cd gesture-snake-game

# 2. Create virtual environment
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate   # Mac/Linux

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the game
python main.py
```

---

## 🎮 Controls

- 👋 Move hand LEFT / RIGHT / UP / DOWN → Control snake  
- 🤏 Pinch (thumb + index finger) → Speed boost  
- 🔄 Show "UP" gesture → Restart game  
- ❌ Press ESC → Exit  

---

## 🧠 How It Works

1. Webcam captures real-time video  
2. MediaPipe detects hand landmarks :contentReference[oaicite:0]{index=0}  
3. Gestures are converted into directions  
4. Game updates snake movement :contentReference[oaicite:1]{index=1}  
5. Pinch gesture activates speed boost  

---

## ⚡ Future Improvements

- Gesture accuracy optimization  
- Multiplayer support  
- Mobile camera integration  
- Web-based version  

---

## 👨‍💻 Developer

**Zeeshan**  
GitHub: https://github.com/zeeshan2204  

---

## 📄 License

MIT License — Free to use
