# ✋ Real-Time Hand Sign Detection (ASL) #

A real-time American Sign Language (ASL) hand sign detection system built using OpenCV and a Keras deep learning model, trained on self-collected hand gesture images.
The project detects hand signs live through a webcam and displays the predicted alphabet in real time.

## 🚀 Project Overview ##

This project focuses on recognizing hand gestures representing ASL alphabets using a webcam.
I collected my own dataset of 300×300 images, trained a Keras model on it, and integrated the trained model with OpenCV for real-time prediction.

## The system: ##

Detects a hand from the live camera feed

Crops and preprocesses the hand region

Classifies the gesture using a trained neural network

Displays the predicted ASL alphabet on screen

## 🧠 Tech Stack ##

Python

OpenCV – real-time image processing

MediaPipe (via CVZone) – hand landmark detection

Keras / TensorFlow – deep learning model

NumPy – numerical operations

All required and compatible library versions are listed in requirements.txt to avoid dependency conflicts.

## 📁 Project Structure ##
HandSignDetection/
│
├── Model/
│   ├── keras_model.h5
│   └── labels.txt
│
├── Data/
│   └── (self-collected training images)
│
├── main.py
├── requirements.txt
└── README.md

## 🖐️ How It Works ##

Webcam captures live video frames

Hand is detected using CVZone’s hand tracking module

The hand region is cropped and resized to 300×300

Image is passed to the trained Keras model

Predicted ASL alphabet is displayed in real time

## ⚙️ Setup & Run ##
pip install -r requirements.txt
python main.py


Make sure your webcam is connected before running the script.

## 🧩 Challenges Faced & How I Solved Them ##

Dependency conflicts between libraries
→ Resolved by identifying compatible versions and maintaining them in requirements.txt

Mismatch between training and inference preprocessing
→ Ensured the same image size and preprocessing pipeline during prediction

Incorrect cropping near image boundaries
→ Fixed using offset-based cropping and padding logic

Real-time debugging issues
→ Continuous testing with live camera input helped stabilize predictions

This project taught me that environment setup and debugging are just as important as model training.

## 📌 Future Improvements ##

Support for more ASL alphabets and words

Improve accuracy with a larger and more diverse dataset

Convert predictions to text or speech output

Optimize performance for low-end systems

🤝 Connect

If you found this project interesting, feel free to ⭐ the repository and connect with me on LinkedIn.

All setup details and dependencies can be found in the repository files.
