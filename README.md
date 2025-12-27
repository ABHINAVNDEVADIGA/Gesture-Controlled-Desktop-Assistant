# 🖐️ Gesture-Controlled Desktop Assistant
  -by ABHINAV N DEVADIGA
### Virtual Mouse & System Control Using Hand Gestures

This project implements a **real-time hand gesture–based desktop control system** using a webcam and computer vision. By leveraging **MediaPipe** for hand landmark detection and **PyAutoGUI** for system interaction, users can control mouse movement, clicks, scrolling, system volume, and screen brightness — **completely touch-free**.

---

## ✨ Key Features

- 🖱️ **Virtual Mouse Control**  
  Move the mouse cursor naturally using hand movements.

- 🖱️ **Mouse Actions**  
  - Single click  
  - Double click  
  - Right click  
  - Drag & drop

- 📜 **Scrolling**  
  Vertical and horizontal scrolling using pinch gestures.

- 🔊 **System Volume Control (Windows)**  
  Increase or decrease system volume using hand gestures.

- 💡 **Screen Brightness Control (Windows)**  
  Adjust display brightness without touching the keyboard.

- 🎥 **Real-Time Processing**  
  Low-latency gesture detection using MediaPipe Hands.

---

## 🛠️ Technologies Used

- **Python**
- **OpenCV** – Camera input & image processing  
- **MediaPipe** – Hand landmark detection  
- **PyAutoGUI** – Mouse & keyboard automation  
- **PyCAW** – System audio control (Windows)  
- **screen-brightness-control** – Brightness adjustment  

---

## 💻 System Requirements

- Windows OS (for volume & brightness control)
- Python **3.8 – 3.10** (recommended)
- Webcam (minimum 720p for best accuracy)

---

## 📦 Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/ABHINAVNDEVADIGA/Gesture-Controlled-Desktop-Assistant.git
cd Gesture-Controlled-Desktop-Assistant
2️⃣ Create & Activate Virtual Environment
python -m venv venv
venv\Scripts\activate

3️⃣ Install Dependencies
pip install opencv-python mediapipe pyautogui screen-brightness-control pycaw comtypes


⚠️ Important:
Run the terminal or VS Code as Administrator for reliable volume and brightness control.

🚀 How to Run
python gesture_controller.py


A webcam window titled “Gesture Controller” will open.

Perform gestures in front of the camera to control the system.

Press ENTER while the window is active to exit.

✋ Gesture Guide

The system differentiates between:

Major Hand → Cursor & system control (Right hand by default)

Minor Hand → Scrolling actions (Left hand by default)

Gesture	Hand	Action
✌️ V-Sign	Major	Move Mouse Cursor
✊ Closed Fist	Major	Left-Click Hold / Drag
☝️ Middle Finger	Major	Left Click
👉 Index Finger	Major	Right Click
✌️🤏 Two Fingers Closed	Major	Double Click
🤏 Pinch (Index + Thumb)	Major	Brightness (X-axis) / Volume (Y-axis)
🤏 Pinch (Index + Thumb)	Minor	Vertical / Horizontal Scroll
🧠 How It Works

Webcam captures real-time video frames

MediaPipe detects hand landmarks

Landmark geometry is converted into gesture states

Gestures are mapped to system actions

PyAutoGUI and PyCAW execute OS-level controls

⚠️ Known Limitations

Designed primarily for Windows

Brightness control depends on display hardware

Requires good lighting conditions

📌 Future Enhancements

Gesture customization UI

Multi-monitor support

Cross-platform brightness handling

Executable (.exe) release

Gesture-based app switching

👨‍💻 Author

Abhinav N Devadiga
Gesture-Controlled Desktop Assistant

🔗 GitHub: https://github.com/ABHINAVNDEVADIGA


---

### ✅ What to do next
```bash
git add README.md
git commit -m "Update README with full project documentation"
git push origin master
