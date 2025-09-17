See The World Through AI – YOLO Object Detection

Watch the demo [here](https://www.youtube.com/watch?v=dQw4w9WgXcQ).

<img width="1919" height="789" alt="image" src="https://github.com/user-attachments/assets/d38ef0c8-5fc8-493c-9740-88227001a4d9" />
<img width="1919" height="762" alt="image" src="https://github.com/user-attachments/assets/9621a13b-4cf9-4094-9230-5c85bde93afc" />


A hands-on project to explore **YOLOv8 object detection** in images, videos, and live webcam feeds, with a **Streamlit web app** for easy interaction.

---

## Project Overview

This project allows you to:

- Detect multiple object classes in **images** and **videos**.
- Perform **real-time detection** via webcam.
- Train YOLO on **custom or sample datasets**.
- Deploy a **Streamlit web app** for interactive detection.
- Upload custom YOLO weights (`.pt`) for inference.

---

## Features

- Detect objects with bounding boxes and confidence scores.
- Real-time webcam detection in Colab.
- Train YOLO on small datasets like `coco128`.
- Streamlit web app with:
  - Image and video uploads
  - Confidence threshold slider
  - Adjustable inference image size
  - Annotated results and detection table
  - Optional custom YOLO weights upload

---

## 🛠️ Installation & Setup

### 1. Clone Repository

```bash
git clone https://github.com/IHRM-AI/Object-Detection--YOLO.git
cd Object-Detection--YOLO
```

2. Install Dependencies
```bash
pip install ultralytics opencv-python-headless matplotlib pillow streamlit pyngrok pandas

```

3. Run Jupyter/Colab Notebook
   
Open Object_Detection.ipynb in Google Colab to execute the project interactively.

5. Run Streamlit App
```bash
streamlit run app_streamlit.py
```
Or use ngrok for public access:

```bash

from pyngrok import ngrok
ngrok.set_auth_token("YOUR_NGROK_AUTH_TOKEN")
public_url = ngrok.connect(8501)
print("Public URL:", public_url)

```

Streamlit Web App

Image Upload: Detect objects in images with bounding boxes.

Video Upload: Detect objects in videos and save annotated output.

Custom Weights: Use your trained YOLO weights.

Detection Table: Shows class, confidence, and bounding box coordinates.

