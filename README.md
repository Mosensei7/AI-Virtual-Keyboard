# Virtual Keyboard with Hand Tracking ⌨️✋

This project implements a Virtual Keyboard using OpenCV, cvzone, and Mediapipe Hand Tracking.
You can type on a digital keyboard by simply moving your hand in front of your webcam – no physical keyboard required!

🚀 Features

Real-time hand tracking with webcam.

Detects fingertip position (index finger) to hover over keys.

Detects "click" action when index and middle fingers come close.

Displays a fully functional QWERTY keyboard layout.

Typed text is displayed live on screen.

Supports physical keypress simulation using pynput.

📂 Project Structure
VirtualKeyboard/
│── main.py             # Main script (the code you shared)
│── README.md           # Project documentation

⚙️ Installation

Clone the repository and install dependencies:

git clone https://github.com/yourusername/VirtualKeyboard.git
cd VirtualKeyboard
pip install -r requirements.txt

requirements.txt
opencv-python
cvzone
mediapipe
numpy
pynput

▶️ Usage

Run the project with:

python main.py

Controls:

Move your index finger to hover over a key.

Tap with index + middle finger (bring them close together) to press the key.

Typed text appears in the purple box at the bottom.

📊 Output

The program displays:

A virtual keyboard on screen.

Highlighted keys when hovered.

Green flash effect when a key is pressed.

Typed text output in a live display box.

Example (screenshot):

🛠️ How It Works

Uses Mediapipe Hand Tracking via cvzone.

Detects finger landmarks.

Tracks index fingertip (id=8) for hover detection.

Checks distance between index (8) and middle finger (12) tips.

If distance < threshold → triggers key press.

Key press is sent to the system using pynput.

✨ Future Improvements

Add support for multiple hands.

Enable special keys (Enter, Space, Backspace).

Add sound feedback for key presses.

Option to switch keyboard layouts (numeric, symbols).

📜 License

This project is licensed under the MIT License.

🔗 Author: Mohsen Ibrahim
