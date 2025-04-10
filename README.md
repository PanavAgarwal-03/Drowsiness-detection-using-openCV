# Drowsiness Detection System 🚗😴

A Python-based real-time drowsiness detection system using OpenCV, Dlib, and facial landmark detection. This system can be used to monitor driver alertness and sound an alarm if signs of drowsiness are detected.

## 🔍 Features
- Real-time video stream analysis using webcam
- Eye Aspect Ratio (EAR) to detect eye closure
- Alarm system triggers when drowsiness is detected
- Visual alerts on the video feed

## 🧠 How It Works
The system detects facial landmarks to identify the eyes, then calculates the **Eye Aspect Ratio (EAR)**. If the EAR drops below a certain threshold for a sustained period, it assumes the person is drowsy and triggers an alarm sound.

## 🛠️ Technologies Used
- Python
- OpenCV
- Dlib (with 68 facial landmark predictor)
- imutils
- SciPy
- Pygame (for playing alarm sound)

## 📁 Project Structure
📦 drowsiness-detection ├── models/ │ └── shape_predictor_68_face_landmarks.dat ├── music.wav ├── drowsiness_detection.py └── README.md


## 🚀 Installation & Setup

1. **Clone the Repository**
```bash
git clone https://github.com/PanavAgarwal-03/Drowsiness-detection-using-openCV.git
cd Drowsiness-detection-using-openCV
```

2. **Install Dependencies**
pip install opencv-python dlib imutils scipy pygame

3. **Download the Pre-trained Facial Landmark Model**
 Place shape_predictor_68_face_landmarks.dat inside the models/ directory.
 Download from: http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2

4. **Add Alarm Sound**
 Ensure you have music.wav in the root directory. This will play when drowsiness is detected


## 🧪 Usage

```bash
python drowsiness_detection.py
```

Press 'q' to quit the application.


## ⚠️ Disclaimer

This is a basic prototype and should not be used in real-life safety-critical environments without further testing and validation.

## 🙌 Acknowledgements

Dlib Library
Adrian Rosebrock - PyImageSearch



