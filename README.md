# Skin Disease Detection & LLM Advisor System

A real-time AI-powered backend system designed to classify skin diseases from images and provide context-aware medical recommendations using Large Language Models (LLMs).

## 🚀 Overview
[cite_start]This project fulfills the AI Engineer technical assessment for Excel Technologies Ltd.[cite: 1, 2]. [cite_start]It features a modular pipeline that integrates Computer Vision for disease detection and Generative AI for structured medical advice[cite: 27, 30].

## 🏗️ Technical Stack
- [cite_start]**Backend**: Python 3.10+, FastAPI [cite: 5]
- [cite_start]**AI/ML**: PyTorch / TensorFlow (EfficientNet/YOLOv8) [cite: 8, 34]
- [cite_start]**LLM**: Gemini Flash / Qwen3-VL [cite: 9]
- [cite_start]**Frontend**: Gradio / Streamlit [cite: 6]
- [cite_start]**Deployment**: Docker [cite: 9, 42]

## 🛠️ Features
- [cite_start]**Image Upload API**: High-performance endpoint for real-time skin analysis[cite: 11, 26].
- [cite_start]**Disease Classification**: Accurate detection of skin conditions using transfer learning[cite: 3, 34].
- [cite_start]**LLM Reasoning**: Generates explanations, next steps, and skincare tips based on detection results[cite: 23, 24, 25].
- [cite_start]**Modular Pipeline**: Clean separation between image preprocessing, classification, and LLM modules[cite: 27].

## 📋 API Reference

### Analyze Skin
`POST /analyze_skin`

**Request:**
Multipart/form-data containing the image file.

**Response:**
```json
{
  "disease": "eczema",
  "confidence": 0.92,
  "recommendations": "Use fragrance-free moisturizers...",
  "next_steps": "Consult a dermatologist for a physical exam.",
  "tips": "Avoid harsh soaps and hot showers."
}
