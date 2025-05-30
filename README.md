# Sign Language Word and Letters Detection through Hand Gestures

A real-time sign language detection system using computer vision and machine learning techniques to recognize and interpret American Sign Language (ASL) hand gestures in live video.

## Project Structure

- `__pycache__/` - Python cache directory
- `virtualenv/` - Virtual environment folder
- `.gitignore` - Specifies intentionally untracked files to ignore
- `palm_movement_detection.py` - Core module for hand detection and tracking using MediaPipe
- `palm_prediction.py` - Script for detecting and analyzing palm positions
- `letter_prediction.py` - Script for detecting and interpreting individual letters
- `word_prediction.py` - Script for detecting and interpreting words
- `palm_movement.csv` - Dataset containing palm movement data
- `README.md` - This documentation file
- `recent_data.pkl` - Pickle file containing recently collected data
- `requirements.txt` - List of Python dependencies
- `sign_hand_gesture_data.csv` - Dataset containing hand gesture data

## Dependencies

This project relies on several Python libraries:

- OpenCV (cv2) - For image processing and computer vision
- Mediapipe - For hand landmark detection
- NumPy - For numerical operations
- pandas - For data manipulation
- scikit-learn - For machine learning algorithms
- gTTS and pygame - For text-to-speech functionality

Install all dependencies using:

```bash
pip install -r requirements.txt
```

## Hand Detection Module

The core of this project is implemented in `palm_movement_detection.py` which provides methods for detecting and tracking hands using MediaPipe:

- `find_hands(img, draw=True)` - Processes an image and optionally draws the hand landmarks
- `find_position(img, draw=True)` - Returns the position of hand landmarks in the image and optionally draws them

The detector can be configured with several parameters:
- `mode` - Determines if the detector runs in video mode or static image mode
- `max_hands` - The maximum number of hands to detect and track
- `detection_con` - Minimum confidence value for hand detection
- `presence_con` - Minimum confidence value for hand landmark presence
- `track_con` - Minimum confidence value for hand landmark tracking

## Usage

1. Run letter detection:
```bash
python letter_prediction.py
```

2. Run word detection:
```bash
python word_prediction.py
```

## Data

The project uses two primary datasets:
- `palm_movement.csv` - Contains palm movement sequences for gesture recognition
- `sign_hand_gesture_data.csv` - Contains hand gesture data for sign language interpretation

## Features

- Real-time hand gesture recognition using webcam
- Letter-by-letter sign language interpretation
- Word-level sign language interpretation
- Text-to-speech conversion of interpreted signs
- Data collection mode to add new gestures and improve model accuracy

## License
