# 👁️ NeuroVision AI

## Multimodal Assistive Navigation System for the Visually Impaired

NeuroVision AI is an AI-powered assistive navigation system designed to help visually impaired individuals navigate indoor and outdoor environments safely. The system combines real-time object detection, depth estimation, multilingual voice alerts, and conversational AI to provide environmental awareness and obstacle guidance.

---

## 🚀 Overview

Visually impaired individuals often face challenges while navigating roads, crowded public spaces, and unfamiliar environments. Existing solutions are frequently expensive, internet-dependent, or limited in functionality.

NeuroVision AI addresses these challenges by providing:

* Real-time object detection
* Distance estimation of obstacles
* Directional guidance (Left, Center, Right)
* Multilingual voice assistance
* Conversational scene understanding
* Cross-device accessibility

The system works directly through a web browser and supports laptops, Android devices, and iPhones without requiring a dedicated mobile application.

---

## ✨ Features

### 🎯 Real-Time Object Detection

* Detects surrounding objects using YOLOv8.
* Identifies obstacles such as vehicles, pedestrians, bicycles, animals, and everyday objects.

### 📏 Depth Estimation

* Uses MiDaS depth estimation to estimate the relative distance of detected objects.
* Provides better environmental awareness for users.

### 📍 Directional Navigation Alerts

* Indicates obstacle position as:

  * LEFT
  * CENTER
  * RIGHT
* Helps users make navigation decisions more safely.

### 🗣️ Multilingual Voice Assistance

Supports:

* English
* Tamil
* Hindi
* Malayalam
* Kannada
* Telugu

### 🤖 Conversational AI

* Ask questions about the current scene using voice or text.
* Provides contextual responses powered by Groq LLaMA 3.

### 📱 Cross-Platform Support

* Laptop Webcam
* Android Smartphones
* iPhones
* No app installation required

### 🌐 Cloud-Based Deployment

* Frontend deployed on Vercel
* Backend deployed on Hugging Face Spaces

---

## 🏗️ System Architecture

```text
Camera Input
      │
      ▼
React Frontend
      │
      ▼
FastAPI Backend
      │
 ┌────┴────┐
 ▼         ▼
YOLOv8   MiDaS
Object   Depth
Detection Estimation
 └────┬────┘
      ▼
Scene Analysis
      │
      ▼
Voice Narration
      │
      ▼
Groq LLaMA 3
Conversational AI
```

---

## 📂 Project Structure

```text
NeuroVision-AI/
│
├── backend/
│   ├── app.py
│   ├── detect.py
│   ├── depth.py
│   ├── narrate.py
│   ├── voice.py
│   ├── chat.py
│   ├── Dockerfile
│   └── requirements.txt
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── App.jsx
│   │   └── components/
│   │       ├── Camera.jsx
│   │       ├── AlertOverlay.jsx
│   │       ├── VoiceChat.jsx
│   │       └── LanguageSelector.jsx
│   └── package.json
│
├── .gitignore
└── README.md
```

---

## 🛠️ Technology Stack

| Component          | Technology          |
| ------------------ | ------------------- |
| Object Detection   | YOLOv8              |
| Depth Estimation   | MiDaS DPT-Small     |
| Conversational AI  | Groq LLaMA 3        |
| Speech-to-Text     | Whisper             |
| Text-to-Speech     | gTTS                |
| Backend Framework  | FastAPI             |
| Frontend Framework | React               |
| Backend Hosting    | Hugging Face Spaces |
| Frontend Hosting   | Vercel              |

---

## ⚙️ Installation

### Backend Setup

```bash
cd backend
pip install -r requirements.txt
python app.py
```

### Frontend Setup

```bash
cd frontend
npm install
npm start
```

---

## 🌐 Deployment

### Frontend

Deploy using Vercel:

* Connect GitHub repository
* Import React project
* Deploy automatically

### Backend

Deploy using Hugging Face Spaces:

* Create a Docker Space
* Upload backend files
* Configure environment variables
* Deploy FastAPI application

---

## 🎯 Applications

* Assistive navigation for visually impaired users
* Accessibility-focused AI systems
* Smart mobility solutions
* Computer vision-based guidance systems
* Human-centered AI applications

---

## 🔮 Future Enhancements

* Custom-trained object detection model
* GPS-assisted navigation
* Offline edge-device deployment
* Emergency assistance integration
* Advanced route planning
* Wearable device integration

---

## 👨‍💻 Author

**Pavithra D**

Artificial Intelligence & Machine Learning Enthusiast

GitHub: https://github.com/Pavithrad-21

---

## 📜 License

This project is developed for educational, research, and accessibility-focused purposes.
