<div align="center">

# AI-Based Truck Tube Counting System

### YOLOv11 + PPO Reinforcement Learning + 3D Structural Counting

<p align="center">
  <img src="screenshots/dashboard.png" width="100%">
</p>

<br>

![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python)
![YOLOv11](https://img.shields.io/badge/YOLOv11-Object%20Detection-black?style=for-the-badge)
![PPO](https://img.shields.io/badge/PPO-Reinforcement%20Learning-red?style=for-the-badge)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green?style=for-the-badge&logo=fastapi)
![Computer Vision](https://img.shields.io/badge/Computer%20Vision-AI-purple?style=for-the-badge)

</div>

---

## Overview

An AI-powered truck tube counting system developed for **Aygaz** as a graduation project by **Can Özel** and **Enes İşbilen** under the supervision of **Ayşe Salman**.

The system combines:

- YOLOv11 Object Detection
- PPO-based Reinforcement Learning
- Adaptive Confidence Threshold Selection
- Multi-view Image Analysis
- Diagonal Traversal Grid Counting
- Explainable AI Dashboard

to estimate the total number of gas cylinders loaded on transport trucks.

Unlike traditional fixed-threshold pipelines, the system dynamically selects the optimal confidence threshold using a Reinforcement Learning agent to improve counting stability across different detection distributions.

---

# System Architecture

<p align="center">
  <img src="assets/architecture.png" width="90%">
</p>

```text
Image Upload
      ↓
YOLOv11 Detection
      ↓
PPO Threshold Selection
      ↓
Adaptive Filtering
      ↓
Diagonal Traversal Counting
      ↓
3D Count Estimation
      ↓
Interactive Dashboard
```

---

# Dashboard Preview

## Main Dashboard

<p align="center">
  <img src="screenshots/dashboard.png" width="100%">
</p>

---

## Detection Visualization

<p align="center">
  <img src="screenshots/detection.png" width="100%">
</p>

---

## PPO Threshold Selection

<p align="center">
  <img src="screenshots/rl-threshold.png" width="100%">
</p>

---

## Confidence Distribution

<p align="center">
  <img src="screenshots/histogram.png" width="100%">
</p>

---

# Key Features

- Adaptive PPO-based threshold selection
- YOLOv11-powered object detection
- Multi-view truck analysis
- Explainable AI visualization
- Confidence analytics
- Structural diagonal traversal counting
- 3D count estimation
- FastAPI-powered inference backend
- Real-time dashboard visualization

---

# Reinforcement Learning Integration

Instead of using a fixed confidence threshold, the system dynamically selects the optimal threshold using a PPO-based Reinforcement Learning agent.

### Candidate Thresholds

```text
25% → 70%
```

The RL agent evaluates:

- confidence distributions
- detection count variations
- confidence statistics

and selects the most suitable threshold for stable counting performance.

---

# 3D Counting Logic

The system performs:

- row-column grid extraction
- diagonal traversal grouping
- layer-based structural estimation

to estimate total cylinder count in stacked truck configurations.

This enables approximate 3D counting from multi-view 2D images.

---

# Example Output

| Metric | Result |
|---|---|
| Grid Structure | 9 × 7 |
| Layer Count | 5 |
| RL Threshold | 55% |
| Estimated Total Count | 315 |

---

# Technologies Used

| Category | Technologies |
|---|---|
| AI / ML | YOLOv11, PPO, Stable-Baselines3 |
| Computer Vision | Roboflow, OpenCV |
| Backend | FastAPI, Uvicorn |
| Frontend | HTML, CSS, JavaScript, Chart.js |
| Deployment | Google Colab, ngrok |
| Programming Language | Python |

---

# Explainable AI Components

The dashboard visualizes:

- RL threshold decisions
- confidence distributions
- detection confidence scores
- diagonal traversal maps
- class distributions

to make the AI inference pipeline more interpretable.

---

# Project Team

### Developers
- Can Özel
- Enes İşbilen

### Supervisor
- Ayşe Salman

### Organization
- Aygaz

---

# Repository Structure

```text
ai-truck-tube-counting/
│
├── README.md
├── LICENSE
│
├── screenshots/
├── docs/
└── assets/
```

---

# Notes

> Source code is not fully public due to project-specific implementation and deployment constraints.

---

# License

MIT License

---

# Contact

### Can Özel

Backend & AI Systems Enthusiast

- LinkedIn: https://linkedin.com/in/YOUR_LINK
- GitHub: https://github.com/YOUR_USERNAME
