PROPOSED SMART MIRROR – RESOLDEPMIRROR
🏗️ Hardware Architecture
The hardware design of ResolDepMirror includes:

Two-way Mirror

LCD Screen

Camera (Raspberry Pi)

Speaker

Mirror and LCD Screen
The two-way mirror provides both transparency and reflectiveness, allowing a digital interface while hiding the underlying hardware. The LCD screen is enclosed inside a wooden box for a seamless appearance.

🖼 Figure - Hardware Architecture
![Hardware Architecture](/hardware_Architecture.png)
 Raspberry Pi
The Raspberry Pi Model 3B is used, featuring:
✔️ 64-bit Quad-Core ARM Cortex-A1 Processor
✔️ 40 GPIO Pins
✔️ SD Card Slot (used as a hard disk)
✔️ USB, Ethernet, Wi-Fi, HDMI, and Camera Serial Interface


 Speaker & Camera
Camera: 12MP camera for emotion detection

Speaker: Plays Quranic verses and guides breathing exercises

 Other Components
SD Card: 32GB (stores OpenCV, TensorFlow, OS)

HDMI Cable: Connects Raspberry Pi to LCD

Power Cable: 5V USB Charger

💻 Software Architecture
The software uses computer vision (OpenCV) and deep learning to train emotion recognition models.

🖼 Figure - Software Architecture
![Software Architecture](/Sofware_Architecture.png)
 Dataset
Primary Data: 270 facial expression images (happy, sad, angry)

Secondary Data: Kaggle dataset

Image Processing & Model Training
Haar Cascade Classifier: Detects facial features

MobileNet Model: Lightweight deep learning model for training datasets (70.9–89.9% accuracy)

Real-Time Emotion Detection
If a user is sad ➝ Quranic verse is displayed & read aloud
If a user is angry ➝ Breathing exercises are shown


⚙️ Functionality of ResolDepMirror
 Sad Mood Module
✔️ Uses Cognitive Behavioral Therapy (CBT) principles
✔️ Displays motivational Quranic verses using Tkinter (GUI)
✔️ Speaks the verse using Google Text-To-Speech (gTTs API)

 Angry Mood Module
✔️ Guides breathing exercises through text & voice

🖼 Figure  - ResolDepMirror Functionality

![Functionality](/Detail_function_of_smart_mirror.png)
📌 4.4 Summary
Hardware: Mirror, LCD, Raspberry Pi, Camera, Speaker

Software: OpenCV, Deep Learning (MobileNet), Emotion Detection

Functionality: Identifies sad/angry moods, responds with Quranic verses or relaxation exercises

📜 Citations
WHO Depression Report (322 Million Affected)

Kaggle Facial Expression Dataset

MobileNet Deep Learning Model
