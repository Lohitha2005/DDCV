Driver Drowsiness Detection 🚗💤
Overview
Driver drowsiness is one of the leading causes of road accidents worldwide. Staying alert behind the wheel is critical, but fatigue and sleepiness can sneak up on even the most experienced drivers.
Our project aims to detect driver drowsiness in real-time using advanced deep learning techniques — ensuring safer journeys and reducing accident risk.
Motivation
Traditional CNN-based methods for detecting drowsiness work, but their accuracy is often limited when handling subtle facial changes like eye closure, yawning, or head tilts.
To overcome this limitation, we implemented an Optimized Convolutional Neural Network (OOCN) that improves detection accuracy, even under challenging conditions like:Low light / night drivingDifferent head poses
Partial face occlusions

Features
✅ Real-time drowsiness detection using webcam feed

✅ Alerts the driver when signs of fatigue are detected

✅ Uses facial landmarks (eyes, mouth) for precise monitoring

✅ Optimized CNN architecture (OOCN) for better accuracy than standard CNN

How It Works

Face Detection: Using a pre-trained shape predictor, we locate the driver’s face.

Feature Extraction: Key facial landmarks (eyes, mouth) are extracted.

Classification: The extracted features are fed into the OOCN model, which predicts alert vs drowsy states.

Alerts: If the driver appears drowsy, an audible and visual alert is triggered instantly.

Why OOCN Over CNN?
Model	Accuracy	Strengths	Weaknesses
CNN	Moderate	Simple, easy to implement	Misses subtle drowsiness signs
OOCN	High	Captures subtle facial cues, robust under different conditions	Slightly more complex

By using OOCN, we boost accuracy and reliability, making the system more practical for real-world driving scenarios.
Installation
# Clone the repository
git clone https://github.com/Lohitha2005/DDCV.git

# Install dependencies
pip install -r requirements.txt

# Run the drowsiness detection
python Drowsiness_Detection.py
Requirements
Python 3.x
OpenCV
dlib
numpy
playsound
TensorFlow / Keras

Demo
https://drive.google.com/file/d/1MP3J_ULM7gG_Iu-oNo_8FxFRHvIXSBS0/view
Future Improvements
Integrate eye-tracking hardware for more precise measurements
Extend detection to multiple drivers in a vehicle
Add mobile and embedded system support

Contributing
We welcome contributions! If you improve accuracy, optimize performance, or add features, feel free to open a pull request.
