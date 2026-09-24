<div align="center">

[![License: All Rights Reserved](https://img.shields.io/badge/License-All%20Rights%20Reserved-red.svg)](LICENSE)
[![Python 3.8+](https://img.shields.io/badge/python-3.8%2B-blue.svg)](https://www.python.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6%2B-f7df1e.svg)](https://www.developer.mozilla.org/en-US/docs/Web/JavaScript)
[![MediaPipe](https://img.shields.io/badge/MediaPipe-Tasks-orange.svg)](https://developers.google.com/mediapipe)
[![OpenCV](https://img.shields.io/badge/OpenCV-Computer%20Vision-green.svg)](https://opencv.org/)

</div>

# Mesh Vision Analyzer

A lightweight, Python-based computer vision tool designed to perform real-time facial mesh landmark detection and spatial semantic analysis using MediaPipe and OpenCV, optimized for interactive execution in Google Colab.

---

## 🚀 Quick Start / Run in Google Colab

You can run the complete end-to-end pipeline (from browser webcam capture and MediaPipe landmarker initialization to real-time spatial HUD rendering) directly in your browser using Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/amirkabirian/Mesh-Vision-Analyzer/blob/main/notebooks/mesh_vision_node.ipynb)

---

## 💡 What This Project Does (Overview)

**Mesh Vision Analyzer** is an interactive computer vision system that captures live video frames directly from your browser, detects precise facial landmark mesh points, and performs instant semantic spatial analysis. 

Its core operational workflow includes:
1. **Webcam Frame Capture:** Renders an interactive browser button via JavaScript execution (`getUserMedia`) to record a live frame from the user's camera.
2. **Mesh Landmarking:** Utilizes Google's MediaPipe `Face Landmarker` model to map precise 2D/3D coordinate points across facial features.
3. **Semantic HUD & Analysis:**
   * **Head Pose Estimation:** Determines directional orientation (frontal, turned left/right, tilted up/down).
   * **Symmetry Scoring:** Evaluates structural balance and geometric ratios across spatial coordinates.
   * **Expression Detection:** Recognizes emotional expressions using blendshape scoring matrices.
4. **Visual Rendering:** Overlays analytical metrics as a Heads-Up Display (HUD) alongside green landmark meshes onto the processed frame and renders it using Matplotlib.

---

## 🛠️ Technology Stack & Languages

This project bridges web integration and machine learning through a multi-technology stack:
* **Python:** The primary backend language handling image processing (`OpenCV`), numerical arrays (`NumPy`), visualization (`Matplotlib`, `Pillow`), and core execution logic.
* **JavaScript:** Executed inside the browser environment via Colab to handle media stream access, permissions, and direct webcam stream handling.
* **MediaPipe (Google Tasks API):** Provides state-of-the-art machine learning models for fast, on-device mesh and spatial tracking.

---

## 📁 Repository Structure

```text
Mesh-Vision-Analyzer/
├── notebooks/          
│   └── mesh_vision_node.ipynb   # Main Jupyter notebook containing the full implementation
├── LICENSE                      # All Rights Reserved License
└── README.md                    # Project documentation
