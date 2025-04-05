
# Real-Time Machine Fault Detection and Classification using Acoustic Data on Raspberry Pi with Deep Learning

This project focuses on building a real-time system for detecting and classifying faults in car engines using acoustic data. The system leverages Deep Learning techniques, specifically Convolutional Neural Networks (CNNs), and is deployed on a Raspberry Pi for edge computing.

## 🔍 Abstract

The goal of this project is to develop a low-cost, real-time machine fault detection system that uses sound data to identify potential malfunctions in vehicles. The system records engine sounds, processes them into spectrograms, and classifies the sounds using a trained CNN model. It aims to assist mechanics and car owners in quickly diagnosing issues, potentially avoiding costly repairs and improving road safety.

## 📌 Features

- Real-time fault detection using audio signals
- Spectrogram generation from raw audio
- CNN-based classification of engine sound types
- Edge deployment on Raspberry Pi
- Low-cost and portable diagnostic tool

## 🛠️ Technologies Used

- Python
- Raspberry Pi 4
- Librosa (audio processing)
- Matplotlib (spectrograms)
- TensorFlow / Keras (deep learning)
- OpenCV (optional, for visualizations)
- Microphone module

## 🔧 Hardware Requirements

- Raspberry Pi 4 (or compatible)
- USB microphone
- SD card (16GB+ recommended)
- Power supply for Raspberry Pi

## 🧠 Model Overview

- Input: Audio recordings of car engine sounds
- Preprocessing: Convert audio to spectrogram
- Model: CNN trained to classify sound into:
  - Normal
  - Engine knocking
  - Bearing fault
  - Valve issue
- Output: Predicted class of sound with confidence score

## 🚀 How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/vehicle-fault-detection.git
   cd vehicle-fault-detection
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Record or upload engine sound:
   ```bash
   python record_audio.py
   ```

4. Generate spectrogram and predict:
   ```bash
   python predict_fault.py --audio sample.wav
   ```

5. Deploy model to Raspberry Pi using saved `.h5` file.

## 📁 Repository Structure

```
📂 vehicle-fault-detection
├── data/                # Audio and spectrogram files
├── models/              # Trained CNN model (.h5)
├── scripts/
│   ├── record_audio.py  # Record audio from mic
│   ├── spectrogram.py   # Generate spectrogram
│   └── predict_fault.py # Load model and classify
├── requirements.txt     # Dependencies
└── README.md            # Project overview
```

## 📊 Results

- Accuracy: ~90% on validation data
- Real-time inference on Raspberry Pi in < 3 seconds
- Successfully detects known faults from recorded audio

## 📝 Future Work

- Expand dataset with more car models and fault types
- Improve model accuracy with data augmentation
- Integrate with mobile app for remote diagnostics
- Real-time streaming and continuous monitoring

## 👨‍💻 Authors


Sallah Udin
sallahudinllc@gmail.com


Let me know if you'd like me to include your real name, GitHub username, or modify anything for better customization.
