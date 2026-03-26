# DR Prediction Frontend Dashboard

This repository contains the premium, AI-powered medical dashboard for Diabetic Retinopathy (DR) analysis.

## Features
- **AI Chatbot**: Real-time interaction with a specialized medical assistant (English & Tamil).
- **Retinal Image Analysis**: Drag-and-drop interface for uploading fundus images.
- **Visual Insights**: Dynamic progression graphs (Past, Present, Future) and heatmaps.
- **Medical Reports**: Automated PDF generation for DR findings.
- **Bilingual Support**: Full UI translation between English and Tamil.
- **Voice Support**: Integrated Text-to-Speech (TTS) for AI recommendations.

## Requirements
This frontend is designed to work with the **VisionCare AI FastAPI Backend**.
The dashboard makes relative API calls to:
- POST `/api/v1/analyze` (Image processing & Grad-CAM)
- POST `/api/v1/chat` (Gemini-powered AI assistant)

## Deployment Note
If you are hosting this frontend on a separate server (e.g., GitHub Pages, Netlify), you must:
1. Update the `fetch` URLs in `index.html` to include the full absolute URL of your running backend.
2. Ensure the backend has **CORS** enabled for your frontend domain.
