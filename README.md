✋ Real-Time Hand Sign Detection (ASL)

A real-time American Sign Language (ASL) hand sign detection system built using OpenCV and a Keras deep learning model, trained on self-collected hand gesture images.
The project detects hand signs live through a webcam and classifies them accurately using a trained neural network.

🚀 Project Overview
This project focuses on recognizing hand gestures representing ASL alphabets in real time.
I collected my own dataset of 300×300 images, trained a Keras model on it, and integrated the model with OpenCV for live inference.

The system:
Detects hands from a webcam feed
Preprocesses the hand region
Classifies the gesture using a trained model
Displays the predicted alphabet live on screen

🧠 Tech Stack
Python
OpenCV – real-time image processing
MediaPipe (via CVZone) – hand landmark detection
Keras / TensorFlow – model training & inference
NumPy – numerical operations

All compatible library versions are listed in requirements.txt to avoid dependency conflicts.

📁 Project Structure
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

🖐️ How It Works
Webcam captures live video
Hand is detected using CVZone
Hand region is cropped and resized to 300×300
Image is passed to the trained Keras model
Predicted ASL alphabet is displayed in real time

⚙️ Setup & Run
pip install -r requirements.txt
python main.py


Make sure your webcam is connected before running the script.

🧩 Challenges Faced & How I Solved Them

Dependency conflicts between TensorFlow, MediaPipe, and OpenCV
→ Solved by carefully selecting compatible versions and documenting them in requirements.txt

Incorrect predictions due to preprocessing mismatch
→ Fixed by matching training image dimensions exactly during inference

Hand cropping issues near image borders
→ Handled using offset-based cropping and padding logic

Live debugging & testing
→ Continuous real-time testing helped refine accuracy and stability

This project taught me that debugging environment issues can be just as challenging as building the model itself.

📌 Future Improvements
Add more ASL alphabets and words
Improve model accuracy with a larger dataset
Convert output to text or speech

Optimize performance for low-end systems

🤝 Connect

If you found this project interesting or helpful, feel free to ⭐ the repo and connect with me on LinkedIn!
