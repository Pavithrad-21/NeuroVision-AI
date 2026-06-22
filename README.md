# 👁 NeuroVision AI

**Multimodal Assistive Navigation for Visually Impaired — Indian Road Edition**

> Real-time object detection + depth estimation + multilingual voice alerts + conversational AI

## Features
- 🎥 Works on laptop webcam, Android & iPhone (no app install)
- 🚗 Fine-tuned for Indian roads (auto-rickshaw, pothole, stray animals)
- 📍 Directional alerts: LEFT / CENTER / RIGHT
- 🌙 Low-light enhancement
- 🗣️ 6 languages: English, Tamil, Hindi, Malayalam, Kannada, Telugu
- 🤖 Ask questions about your live scene (voice or text)
- 📱 QR code to instantly use phone camera

## Project Structure
```
neurovision/
├── backend/            ← FastAPI (deploy on HuggingFace Spaces)
│   ├── app.py          Main API server
│   ├── detect.py       YOLOv8n detection
│   ├── depth.py        MiDaS depth estimation
│   ├── narrate.py      Multilingual scene narration
│   ├── voice.py        gTTS + Whisper
│   ├── chat.py         Groq LLaMA 3 conversational AI
│   ├── Dockerfile      HF Spaces deployment
│   └── requirements.txt
├── frontend/           ← React app (deploy on Vercel)
│   ├── src/
│   │   ├── App.jsx
│   │   └── components/
│   │       ├── Camera.jsx
│   │       ├── AlertOverlay.jsx
│   │       ├── VoiceChat.jsx
│   │       └── LanguageSelector.jsx
│   └── public/
├── train_colab.py      ← Google Colab fine-tuning notebook
└── SETUP_GUIDE.md      ← Full setup instructions
```

## Tech Stack (100% Free)
| Component | Technology |
|-----------|-----------|
| Object Detection | YOLOv8n (fine-tuned) |
| Depth Estimation | MiDaS DPT-Small |
| Speech-to-Text | OpenAI Whisper |
| Text-to-Speech | gTTS |
| Conversational AI | Groq + LLaMA 3 |
| Backend | FastAPI |
| Frontend | React |
| Backend Hosting | HuggingFace Spaces |
| Frontend Hosting | Vercel |
| Training | Google Colab |
