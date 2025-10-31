# Stickman Hook Gesture Controller

A real-time hand gesture controller for the Stickman Hook game using computer vision and hand tracking. Play Stickman Hook using your webcam and hand gestures, instead of keyboard inputs!

---

## 🎮 Overview

This project allows you to:
- Use two or more fingers to **hook/swing** in the game
- Use one finger or a fist to **release** and fly
- Play in real-time with your webcam and see visual feedback on-screen

## 🛠️ Technologies Used

- OpenCV (`cv2`) for webcam and image processing
- **CVZone** HandTrackingModule (MediaPipe based) for finger detection
- **PyAutoGUI** for keyboard automation
- Python 3.7+

## 🚀 Installation & Setup

1. **Clone this repo:**  
   `git clone <your-repo-url>`
2. **Install dependencies:**  
   `pip install -r requirements.txt`
3. **Open the Stickman Hook game** in your browser or as a desktop game.
4. **Run the controller script:**  
   `python stickmanHook.py`

## 📋 Usage Instructions

- Position your hand in front of your webcam.
- **Show 2+ fingers:** Hook/Swing (holds spacebar in-game)
- **Show 1 finger or a fist:** Release (releases spacebar)
- **Controls:**  
  - `'q'`: Quit application  
  - `'r'`: Reset controller state  
  - *Move mouse to top-left corner* for emergency stop (PyAutoGUI failsafe)
- Ensure good lighting & face camera for best detection.

## 🧩 Customization

- To adjust detection sensitivity or camera resolution, edit config variables at the top of `stickmanHook.py`.
- Change the `HOOK_KEY` variable if your game uses a key other than spacebar.

## 🐛 Troubleshooting

- If camera isn't detected, check permissions and that no other app is using your webcam.
- For detection issues, improve lighting or clean your camera lens.
- If game doesn't respond, ensure its window is active and uses the expected key input.

## 🙏 Credits

- Uses [CVZone](https://github.com/cvzone/cvzone) 
- Thanks to the AIML Club, inspiration from Reinforce Club SST Build Day

Have fun swinging Stickman with your gestures! 🎮✋
