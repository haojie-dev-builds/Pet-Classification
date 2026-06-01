# Face Authentication and Pet Breed Classification System

## Overview
This project is a computer vision-based desktop application that combines **face authentication** and **pet breed classification** into a single user-friendly system.

The application first verifies the user's identity through facial recognition. Once authentication is successful, the user can access a pet breed identification module that classifies either dog or cat breeds from uploaded images or live camera captures.

The system is implemented using Python, OpenCV, TensorFlow Lite, Dlib, and Tkinter.

---

## Features

### Face Authentication

* Real-time webcam face detection
* Face embedding extraction using Image Embeddings
* Similarity matching against authorized users
* Multi-frame verification to improve reliability
* Authentication success/failure tracking

### Dog Breed Classification

* TensorFlow Lite optimized model
* Upload image from local storage
* Capture image directly from webcam
* Displays Top-3 predicted dog breeds with confidence scores

### Cat Breed Classification

* TensorFlow Lite optimized model
* Upload image from local storage
* Capture image directly from webcam
* Displays Top-3 predicted cat breeds with confidence scores

### User Interface

* Modern Tkinter-based graphical interface
* Real-time camera preview
* Interactive navigation between modules
* Image preview before classification

---

## Technologies Used

* Python
* OpenCV
* TensorFlow Lite
* Dlib
* NumPy
* Pillow (PIL)
* Tkinter
* Image Embeddings (imgbeddings)

---

## System Workflow

1. User launches the application.
2. Face authentication starts using the webcam.
3. The captured face is compared against authorized face embeddings.
4. Upon successful authentication:

   * User chooses either Dog Breed Identification or Cat Breed Identification.
5. User uploads an image or captures one using the webcam.
6. The selected TensorFlow Lite model performs breed classification.
7. Top predictions and confidence scores are displayed.

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/face-auth-pet-classification.git
cd face-auth-pet-classification
```

### Install Dependencies

```bash
pip install opencv-python
pip install pillow
pip install numpy
pip install tensorflow
pip install dlib
pip install imgbeddings
pip install psutil
```

---

## Running the Application

```bash
python main.py
```

Ensure the following files are available before running:

* dog_breed_model.tflite
* cat_breed_model.tflite
* db_faces.npy
* shape_predictor_68_face_landmarks.dat
* dog_class_indices.pkl
* cat_class_indices.pkl

---

## Future Improvements

* Support additional pet species
* User registration for new authorized faces
* Cloud database integration
* Mobile application deployment
* Improved face anti-spoofing mechanism
* Real-time pet breed detection from video streams

---

## Author

Developed as a Computer Vision and Machine Learning project demonstrating biometric authentication and pet breed classification using deep learning models.
