# ai-jewelry-authentication

💎 AI Jewelry Authentication System (7B VLM)

An AI-powered jewelry verification system that compares two jewelry images and generates a precise similarity score (0–100) using a quantized 7B Vision-Language Model.

📌 Overview

This system uses a state-of-the-art Vision-Language Model (Qwen 2.5 VL 7B) to:

🔍 Analyze jewelry images
🧠 Understand structure & design
📊 Compute similarity score
🚨 Detect mismatches or fraud

Built for:

Jewelry authentication
Fraud detection
Marketplace verification
E-commerce quality control

🚀 Key Features

🧠 AI-Based Comparison
Uses Qwen2.5-VL-7B-Instruct
Deep visual + semantic understanding

📊 Smart Similarity Scoring

Outputs score (0–100)
Based on:
Shape
Structure
Stones
Metal type
Design symmetry

🔥 Advanced Rule-Based Prompting

Strict scoring rules for consistency
Eliminates bias from:
Lighting
Background
Camera quality

⚡ Optimized for Low VRAM

4-bit quantization (BitsAndBytes)
Runs on Kaggle GPU

🖼️ Dual Image Upload UI

Upload 2 images
Drag & drop support
Instant scoring

🏗️ System Architecture

User Upload (2 Images)
        ↓
Gradio Frontend UI
        ↓
Image Preprocessing (Resize 1024x1024)
        ↓
Qwen2.5-VL 7B Model (Quantized)
        ↓
Prompt-based Reasoning Engine
        ↓
Similarity Score (0–100)

⚙️ Tech Stack

AI Model: Qwen2.5-VL-7B-Instruct
Framework: Transformers (HuggingFace)
Quantization: BitsAndBytes (4-bit)
Frontend: Gradio
Backend: Python (PyTorch)
Deployment: Kaggle / Hugging Face Spaces

📸 UI Preview

Your system interface includes:

Image upload panels
Similarity score output
Submit & clear buttons

🧠 Model Details

Model: Qwen/Qwen2.5-VL-7B-Instruct
Quantization: 4-bit NF4
Device: GPU (Auto device mapping)

👉 Model loading & setup:


🧪 How It Works

Step-by-Step Logic:
Image Upload
Resize to 1024x1024
Prompt injected into VLM
Model compares images
Strict scoring rules applied
Final score returned

🧠 Scoring Intelligence

The model follows structured reasoning:

Jewelry type check
Silhouette comparison
Structure analysis
Material verification
Fine feature scoring

📊 Example Output
92

🚀 Setup Instructions

1️⃣ Install Dependencies
pip install transformers accelerate bitsandbytes pillow gradio

2️⃣ Run the App
python app.py

3️⃣ Open UI
http://127.0.0.1:7860

🖥️ Usage
Upload Image 1
Upload Image 2
Click Submit
View similarity score

⚡ Performance Optimization

4-bit quantization reduces VRAM usage
max_new_tokens reduced for speed
use_cache=False for stability
GPU memory cleared after inference

🔐 Limitations

Requires GPU for best performance
Large model (7B parameters)
Internet required for model download

📈 Future Enhancements

🗺️ Bounding box detection
🔍 Object segmentation
📊 Explainable AI (visual heatmaps)
📱 Mobile app integration
☁️ Cloud deployment (AWS / GCP)

👨‍💻 Author

Developed as part of an AI-powered Visual Authentication System

📜 License

MIT License

⭐ Support

If you like this project:

⭐ Star the repo
🍴 Fork it
🚀 Share with others
