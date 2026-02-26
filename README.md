🎧 Gesture-Based AI DJ Controller

A real-time, touchless DJ controller that uses computer vision to map hand gestures to audio controls. The system allows mixing and blending of two songs while adjusting volume, vocals, bass, and treble using natural hand movements captured via a webcam.

This project combines OpenCV + MediaPipe for hand tracking, Demucs for AI-based vocal separation, and Tkinter for a live interactive UI.

<img width="2048" height="1154" alt="image" src="https://github.com/user-attachments/assets/1374ea99-f72e-4c6a-9aa2-e3b3657fbcd9" />

✨ Features

Real-time two-hand gesture control

AI-based vocal separation using Demucs (cached after first run)

Touchless control of:

Volume

Vocal mix

Bass

Treble

Gesture-based track navigation (next / previous)

Play / pause using both hands

Live UI feedback synced with gestures

🎮 Gesture Controls
🖐️ Right Hand

Rotate hand → Volume control

Move up / down → Vocal level

Close fist → open → Next track

🤚 Left Hand

Rotate hand → Bass control

Move up / down → Treble control

Close fist → open → Previous track

👊 Both Hands

Close both fists → Play / pause toggle

🛠️ Tech Stack

Python

OpenCV

MediaPipe

Demucs (HTDemucs model)

PyAudio

Librosa

Tkinter

🚀 How to Run

Clone the repo

git clone https://github.com/your-username/gesture-dj-controller.git
cd gesture-dj-controller

Install dependencies

pip install -r requirements.txt

Add audio files
Place .mp3 or .wav files inside the music/ folder.

Run the app

python "Addapt DJ software with interface.py"

⚠️ Note:
First-time vocal separation may take 30–90 seconds per track. Separated files are cached for faster playback later.

📁 Project Structure
gesture-dj-controller/
├── assets/
│   └── demo-ui.png
├── music/
├── separated/
├── Addapt DJ software with interface.py
└── README.md
⚠️ Limitations & Notes

Vocal separation is performed using Demucs and is computationally heavy

No beat matching or BPM sync (not a full professional DJ system)

Gesture recognition uses rule-based logic, not ML classification

Designed as an experimental prototype for gesture-based interaction

📌 Future Improvements

Split code into modular files

Add beat matching / crossfade control

Improve gesture robustness under low lighting

Add configurable gesture mappings

📜 License

This project is for educational and experimental purposes.
