**🎵 Emotion-Based Music Player System (Django Project)**
A smart web application that detects human emotion using face and audio analysis, then recommends and plays music based on the recognized emotional state. Built using Django, OpenCV, Keras, BERT, and audio feature extraction libraries.

**🧾 Project Overview**
This system analyzes facial expressions and audio speech inputs to determine the user's emotional state. Once detected, it automatically recommends and plays songs aligned with that emotion — enhancing user experience through emotional AI and multimedia interaction.

**🧠 Core Technologies Used**
Django Framework for web development

OpenCV for face detection

Keras and CNN for image-based emotion detection

Librosa and SoundFile for audio feature extraction

Sentence-BERT for understanding emotional text

Multiprocessing & Playsound for asynchronous music playback

Base64 & File Handling for image uploads via webcam

🖥️ Modules & Functionality
🔹 Emotion Detection (Face-based)
Captures image from webcam or uploaded file

Detects faces using Haar Cascade Classifier

Crops and resizes detected face

Classifies emotion using a trained CNN model

🔹 Emotion Detection (Audio-based)
Extracts MFCC, Chroma, and Mel features from .wav file

Recognizes emotions such as happy, sad, angry, scared, surprise, etc.

🔹 Emotion Detection (Text-based)
Uses Sentence-BERT to encode and understand emotional context from input text

🔹 Music Recommendation System
Based on predicted emotion, recommends relevant songs

Automatically populates a list of playable songs

Plays selected song using a multiprocessing audio player

🔹 Play / Stop Controller
Allows user to play music in a new tab

Option to stop the current playback

**🗂️ Project Structure Overview**
EmotionApp/ – Django App folder

static/photo/ – Stores temporary user face images

model/ – Contains Haar Cascade, CNN model, weights, and other emotion-related models

songs/ – Organized by emotion category (e.g., happy, sad, angry) with related music files

templates/ – HTML pages (index.html, VideoChatbot.html) for UI

views.py – Core logic for detecting emotion, managing webcam, recommending and playing songs

**🧪 Emotions Supported**
Facial & Audio Emotions:

Angry

Disgust

Scared

Happy

Neutral

Sad

Surprise

Text-based Emotions:

Sad

Happy

Neutral

Angry

Scared

Surprise
**
📸 How It Works**
The user opens the web app.

Uploads or captures an image via webcam OR submits speech/text input.

The system predicts the dominant emotion.

A customized list of songs is displayed based on the predicted emotion.

User clicks a song to start playback in a separate process.

Option to stop music anytime.

**🎯 Use Cases**
Mood-based music recommendation

Smart entertainment applications

Emotion-aware digital interfaces

Assistive tools for mental wellness

