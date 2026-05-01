# AI Surroundings Guide

A computer vision and AI-powered web application designed as an assistive tool for the visually impaired. It uses your device's camera to analyze the surroundings and provides a natural, spoken description of the scene using Text-to-Speech.

## Features
- **Real-time Object Detection:** Uses YOLOv8 to quickly identify objects, their direction, and proximity.
- **Natural Language Descriptions:** Integrates with Llama vision models via Groq to generate intuitive, human-like scene descriptions.
- **Instant Audio Feedback:** Uses browser-native Text-to-Speech to instantly read descriptions aloud to the user.
- **Mobile-Friendly UI:** A sleek, dark-mode interface that feels like a native app.

## Tech Stack
- **Backend:** FastAPI, Python, Ultralytics (YOLOv8), OpenAI SDK (via Groq).
- **Frontend:** HTML, CSS, JavaScript (Browser Native Speech API).
- **Deployment Ready:** Configured with `Procfile` and `Dockerfile` for easy deployment on Render, Railway, or Hugging Face.

## Local Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Ronxak/AI-Surroundings-Guide.git
   cd AI-Surroundings-Guide
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Environment Variables:**
   Rename `.env.example` to `.env` and add your Groq API Key:
   ```env
   GROQ_API_KEY=your_api_key_here
   ```

4. **Run the app:**
   ```bash
   uvicorn app.main:app --reload
   ```

5. **Access the application:**
   Open your browser and navigate to `http://localhost:8000/`
