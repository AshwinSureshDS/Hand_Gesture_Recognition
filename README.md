# Hand Gesture Recognition

This project implements a real-time hand gesture recognition system using computer vision and machine learning techniques. It can detect and classify various hand gestures through a webcam feed.

## Features

- Real-time hand tracking and gesture recognition
- Support for 10 different hand gestures:
  - Okay
  - Peace
  - Thumbs up
  - Thumbs down
  - Call me
  - Stop
  - Rock
  - Live long
  - Fist
  - Smile
- Visual feedback with hand landmark visualization

## Requirements

- Python 3.6+
- Webcam
- Required libraries (see requirements.txt)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/Hand-Gesture-Recognition.git
   cd Hand-Gesture-Recognition
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

Run the main script to start the hand gesture recognition:

```
python hg.py
```

The webcam feed will open, showing your hand with landmarks. The recognized gesture will be displayed in the top-left corner of the window.

- Press 'q' to quit the application

## How It Works

The system uses the following components:

1. **OpenCV**: For capturing and processing video frames
2. **MediaPipe**: For hand landmark detection
3. **TensorFlow**: For gesture classification using a pre-trained model

The pipeline works as follows:
1. Capture video frames from the webcam
2. Detect hand landmarks using MediaPipe
3. Extract landmark coordinates as features
4. Classify the gesture using a pre-trained model
5. Display the result on the screen

## Jupyter Notebook

The repository includes a Jupyter notebook (`hand_gesture_recognition.ipynb`) that demonstrates the development process and allows for experimentation with the code.

## License

This project is licensed under the MIT License - see the LICENSE file for details.