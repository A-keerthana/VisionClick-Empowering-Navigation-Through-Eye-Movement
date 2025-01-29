
# VisionClick: Empowering Navigation Through Eye Movement

## Eye-controlled Mouse Python Project

### Overview
This project implements an **eye-controlled mouse** using OpenCV, MediaPipe, and PyAutoGUI. The system tracks eye movements using facial landmarks and translates them into cursor movements and clicks. This allows users to control their computer using only their eye movements.

### Features
- Tracks eye movements using **MediaPipe FaceMesh**.
- Moves the mouse cursor based on eye position.
- Detects eye blinking to simulate mouse clicks.
- Uses **OpenCV** for real-time video processing.
- Works with any standard webcam.

### Installation

#### Prerequisites
Ensure you have Python installed on your system (Python 3.7 or higher is recommended).

#### Install Required Libraries
Run the following command to install the required dependencies:

```bash
pip install opencv-python mediapipe pyautogui
```

### Usage
1. Connect a webcam to your system.
2. Run the script:
   ```bash
   python main.py
   ```
3. A window will open displaying the webcam feed.
4. Move your eyes to move the cursor.
5. Blink to perform a click.

### How It Works
- The script captures video frames using OpenCV.
- **MediaPipe FaceMesh** detects facial landmarks.
- Specific eye landmarks (indices **474-478**) are used to track eye movement.
- The **cursor position** is updated based on eye gaze.
- The script detects **eye blinks** (difference in vertical eye landmarks) to trigger a mouse click.

### File Structure
```
📂 VisionClick-Empowering-Navigation-Through-Eye-Movement
 ├── 📂 Eye-controlled-MousePythonProject
 │    ├── main.py  # Main script for eye-controlled mouse
 │    ├── README.md  # Project documentation
```

### Dependencies
- Python 3.7+
- OpenCV
- MediaPipe
- PyAutoGUI

### Future Improvements
- Improve gaze tracking accuracy.
- Implement calibration for different users.
- Support additional gestures for scrolling and right-click.
- Optimize performance for different lighting conditions.

### Troubleshooting
#### 1. Webcam Not Detected
- Ensure your webcam is properly connected.
- Check if another application is using the webcam.

#### 2. Cursor Not Moving
- Ensure your face is properly visible in the webcam.
- Try adjusting the lighting conditions.

#### 3. Blinking Not Registering as Click
- Adjust your blinking speed.
- Ensure your face is fully within the frame.

### Author
Developed by **A-keerthana**.

### License
This project is open-source and available under the MIT License.

