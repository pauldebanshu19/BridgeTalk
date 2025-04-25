# Sign Language Detection System

A real-time sign language detection system using Mediapipe and TensorFlow. This project can detect basic sign language gestures including 'hello', 'thanks', and 'iloveyou'.

## Features

- Real-time sign language detection using webcam
- Detection of three basic signs:
  - Hello
  - Thanks
  - I Love You
- Visual feedback with landmark tracking
- LSTM-based gesture recognition
- Easy to use interface

## Requirements

- Python 3.8 or higher
- TensorFlow 2.8.0 or higher
- OpenCV 4.5.0 or higher
- Mediapipe 0.8.9 or higher
- NumPy 1.19.0 or higher

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ActionDetectionforSignLanguage.git
cd ActionDetectionforSignLanguage
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Run the sign language detection script:
```bash
python sign_language_detection.py
```

2. The webcam will open and start detecting signs in real-time
3. Perform one of the following signs:
   - Hello
   - Thanks
   - I Love You
4. The detected sign will appear at the top of the screen
5. Press 'q' to quit the application

## Project Structure

```
ActionDetectionforSignLanguage/
├── sign_language_detection.py  # Main detection script
├── action.h5                   # Trained model weights
├── requirements.txt            # Project dependencies
└── README.md                   # Project documentation
```

## How It Works

1. The system uses Mediapipe to detect and track:
   - Face landmarks
   - Pose landmarks
   - Hand landmarks
2. These landmarks are processed by an LSTM model
3. The model predicts which sign is being performed
4. Results are displayed in real-time on the screen

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Mediapipe for the landmark detection
- TensorFlow for the machine learning framework
- OpenCV for computer vision capabilities 