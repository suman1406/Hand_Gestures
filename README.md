# Hand Gesture Recognition

This project uses OpenCV and MediaPipe to perform real-time hand gesture recognition. The script captures video from the webcam, detects hands in the video stream, and draws landmarks on the detected hands.

## Project Structure

- **gestures.py**: The main script for capturing video, detecting hands, and drawing landmarks using MediaPipe and OpenCV.

## Requirements

- Python 3.x
- OpenCV
- MediaPipe

## Setup Instructions

1. **Clone the repository**:
    ```bash
    git clone https://github.com/suman1406/Hand_Gestures.git
    ```

2. **Install dependencies**:
    ```bash
    pip install opencv-python mediapipe
    ```

3. **Run the script**:
    ```bash
    python gestures.py
    ```

## Usage

- **gestures.py**:
    - Captures video from the default webcam.
    - Uses MediaPipe to detect hand landmarks.
    - Draws the detected landmarks on the video frame.

## Key Functions

- **cv2.VideoCapture(0)**: Captures video from the default webcam.
- **mp.solutions.hands.Hands()**: Initializes the MediaPipe Hands solution.
- **hands.process(frame_rgb)**: Processes the video frame to detect hand landmarks.
- **mp.solutions.drawing_utils.draw_landmarks**: Draws the detected landmarks on the video frame.