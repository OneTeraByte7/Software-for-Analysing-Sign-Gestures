# 🤟 Sign Language Recognition with Live Text & Audio | OpenCV + TensorFlow
---
## Badges

![OpenCV](https://img.shields.io/badge/OpenCV-%3E=4.0-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%3E=2.x-orange.svg)
![Project Year](https://img.shields.io/badge/Year-2024-green.svg)
[![trophy](https://github-profile-trophy.vercel.app/?OneTeraByte7=ryo-ma&theme=onedark)

A real-time Sign Language Recognition system using computer vision and deep learning. This project detects hand gestures from a webcam feed using OpenCV and classifies them using a trained TensorFlow model. The recognized sign is then displayed as text and spoken aloud using text-to-speech synthesis.

---

## ✨ Features

- 📷 Real-time hand gesture detection via webcam
- 🤖 CNN-based sign language classifier (TensorFlow)
- 💬 Live on-screen text display of predicted sign
- 🔊 Audio output using Text-to-Speech (TTS)
- 🧠 Custom trained model for ASL/Fingerspelling
- ✅ Minimal setup – just install dependencies and run
- 🛠️ Modular scripts for training, inference, and UI

---

## 📁 Project Structure

```bash
  sign-language-recognition/
├── dataset/ # Contains preprocessed gesture images
├── model/ # Saved model (.h5 / .pb)
├── utils/ # Helper functions
├── train.py # Train the model
├── predict.py # Predict from image or webcam
├── live_text_audio.py # Real-time webcam + text + audio output
├── requirements.txt # All Python dependencies
└── README.md # You're here
```


---

## 🚀 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/yourusername/sign-language-recognition.git
cd sign-language-recognition
```

### 2. Install Requirements
Make sure Python 3.7+ is installed.

```bash
  pip install -r requirements.txt
```

### 3. Run the Application
a. To train the model:

```bash
  python train.py
```

b. To test from image or webcam:
```bash
python predict.py
```

c. To launch live recognition with text and audio:
```bash
  python live_text_audio.py
```
---

## 🔧 Requirements

OpenCV ≥ 4.0
TensorFlow ≥ 2.0
NumPy
pyttsx3 (for audio output)
Any working webcam
All dependencies are listed in requirements.txt.

---

## 🧠 Model Detail

Input: Preprocessed hand sign images (grayscale or RGB)
Architecture: CNN with 2-3 Conv layers, ReLU, MaxPooling, Dense
Output: Softmax for multi-class classification (A-Z)
You can easily modify the architecture in train.py.

---

