````markdown
# ✈️ AeroSense
### AI-Powered Predictive Maintenance and Real-Time Telemetry Analysis System for NASA Turbofan Jet Engines Using XGBoost & Explainable AI

<p align="center">

![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-009688?style=for-the-badge&logo=fastapi)
![React](https://img.shields.io/badge/React-Frontend-61DAFB?style=for-the-badge&logo=react)
![XGBoost](https://img.shields.io/badge/XGBoost-MachineLearning-orange?style=for-the-badge)
![SHAP](https://img.shields.io/badge/Explainable-AI-success?style=for-the-badge)
![WebSocket](https://img.shields.io/badge/WebSocket-RealTime-red?style=for-the-badge)
![Docker](https://img.shields.io/badge/Docker-Deployment-2496ED?style=for-the-badge&logo=docker)

</p>

---

# 🌍 Overview

AeroSense is an **AI-powered Predictive Maintenance Platform** that estimates the **Remaining Useful Life (RUL)** of NASA Turbofan Jet Engines using Machine Learning and Explainable AI.

Unlike traditional predictive maintenance projects that only provide offline predictions, AeroSense delivers a complete cloud-ready intelligent monitoring ecosystem featuring:

- ✈️ AI-powered RUL Prediction
- 📡 Real-Time Telemetry Streaming
- 🧠 Explainable AI (SHAP)
- 📊 Interactive Dashboard
- 🚨 Smart Alert System
- ⚙️ Component Health Monitoring
- 🤖 Gemini AI Maintenance Assistant
- ☁️ Dockerized Cloud Deployment

The platform transforms raw aircraft sensor data into actionable maintenance decisions, helping engineers reduce maintenance costs, improve safety, and increase aircraft availability.

---

# 📑 Table of Contents

- Overview
- Features
- Architecture
- Workflow
- Dataset
- Machine Learning Pipeline
- Explainable AI
- Real-Time Monitoring
- Tech Stack
- Folder Structure
- Installation
- API Endpoints
- Results
- Future Enhancements
- Team
- License

---

# 🚀 Features

## 🤖 AI-Based Remaining Useful Life Prediction

Predicts the Remaining Useful Life (RUL) of turbofan engines using state-of-the-art Machine Learning.

### Highlights

- XGBoost Regression
- High Prediction Accuracy
- Fast CPU Inference
- Production Ready
- Real-time Predictions

---

## 🧠 Explainable Artificial Intelligence

Every prediction is completely transparent.

SHAP explains

- Which sensors affected the prediction
- Positive contributions
- Negative contributions
- Sensor importance
- Feature ranking

Available SHAP Visualizations

- Beeswarm Plot
- Waterfall Plot
- Force Plot
- Decision Plot
- Dependence Plot
- Feature Importance Plot

---

## 📡 Live Telemetry Streaming

Using WebSockets, AeroSense continuously streams

- Engine Cycles
- Sensor Values
- Component Health
- Remaining Useful Life
- Engine Status
- Failure Alerts

without refreshing the webpage.

---

## ⚙️ Component Health Monitoring

Tracks the health of

- 🌀 Fan
- 🔥 High Pressure Compressor
- 🔥 Combustor
- 🌪 High Pressure Turbine
- 💨 Low Pressure Turbine
- 🌬 Bypass System

Each component has an independent health score.

---

## 🚨 Intelligent Alert Center

Automatically detects

- Critical Failures
- Sensor Anomalies
- Low Component Health
- High Failure Risk

Alerts are generated in real time.

---

## 🤖 Gemini AI Pilot

Integrated Google Gemini AI allows engineers to ask

- Why did RUL decrease?
- Which sensor caused the issue?
- Explain SHAP values.
- Suggest maintenance.
- Interpret engine health.

---

## 📊 Dashboard

Modern React Dashboard provides

- Live RUL Gauge
- Sensor Charts
- Heatmaps
- SHAP Graphs
- Alert Center
- Engine History
- Maintenance Logs
- AI Chat Assistant

---

# 🏗 System Architecture

```text
                     React Frontend
                           │
          ┌────────────────┴────────────────┐
          │                                 │
     REST APIs                       WebSockets
          │                                 │
          └────────────────┬────────────────┘
                           │
                    FastAPI Backend
                           │
      ┌──────────────┬──────────────┬──────────────┐
      │              │              │
   XGBoost       SHAP Engine    Gemini AI
      │              │              │
      └──────────────┴──────────────┘
                           │
                      SQLite Database
```

---

# 🔄 Complete Workflow

```text
NASA Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Feature Engineering
      │
      ▼
Feature Scaling
      │
      ▼
Model Training
      │
      ▼
Model Evaluation
      │
      ▼
Best Model Selection
      │
      ▼
SHAP Explainability
      │
      ▼
FastAPI Backend
      │
      ▼
React Dashboard
      │
      ▼
Real-Time Monitoring
```

---

# 📂 Dataset

Dataset Used

**NASA C-MAPSS FD001**

Contains

- 100 Aircraft Engines
- Run-to-Failure Records
- 21 Sensor Measurements
- 3 Operational Settings
- Flight Cycles

Target Variable

Remaining Useful Life (RUL)

---

# 🧹 Data Preprocessing

- Missing Value Handling
- Constant Sensor Removal
- Feature Selection
- MinMax Scaling
- RUL Calculation
- RUL Capping at 125
- Train/Test Split

---

# 🤖 Machine Learning Models

| Model | Purpose |
|--------|----------|
| XGBoost | Final Model |
| Random Forest | Baseline |
| LightGBM | Fast Gradient Boosting |
| Gradient Boosting | Ensemble Learning |
| Stacking Regressor | Meta Learner |

---

# 🏆 Best Performing Model

## XGBoost

| Metric | Score |
|---------|--------|
| RMSE | **19.06** |
| MAE | **14.27** |
| R² Score | **0.7445** |
| Training Time | **1.68 Seconds** |

Why XGBoost?

- Highest Accuracy
- Fastest Inference
- CPU Friendly
- Robust
- Easy Deployment

---

# 🧠 Explainable AI

AeroSense doesn't simply predict.

It explains every prediction.

Available Explainability

- SHAP Beeswarm
- SHAP Waterfall
- SHAP Force
- SHAP Decision
- SHAP Dependence
- Feature Importance

Benefits

- Transparent AI
- Regulatory Compliance
- Engineer Trust
- Better Decision Making

---

# 📡 Real-Time Monitoring

WebSocket streams

- Sensor Data
- RUL
- Component Health
- Alerts
- Flight Cycles
- Anomalies

Everything updates live.

---

# 🛠 Tech Stack

## Frontend

- React
- Vite
- Tailwind CSS
- Recharts

## Backend

- FastAPI
- Python
- JWT Authentication
- WebSocket

## Machine Learning

- XGBoost
- Random Forest
- LightGBM
- Gradient Boosting
- Scikit-learn
- SHAP

## Database

SQLite

## Deployment

- Docker
- Render

## AI

Google Gemini API

---

# 📁 Project Structure

```text
AeroSense
│
├── frontend
│   ├── components
│   ├── pages
│   ├── charts
│   ├── dashboard
│   └── authentication
│
├── backend
│   ├── app.py
│   ├── websocket.py
│   ├── database.py
│   ├── alerts.py
│   ├── authentication.py
│   └── telemetry.py
│
├── models
│   ├── xgb_model.pkl
│   ├── rf_model.pkl
│   ├── lgbm_model.pkl
│   ├── ensemble_model.pkl
│   └── scaler.pkl
│
├── dataset
├── shap
├── docker
└── README.md
```

---

# ⚙ Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/AeroSense.git
```

Backend

```bash
cd backend

pip install -r requirements.txt

uvicorn app:app --reload
```

Frontend

```bash
cd frontend

npm install

npm run dev
```

---

# 📡 API Endpoints

| Method | Endpoint | Description |
|----------|----------------|----------------------------|
| POST | /predict | Predict Remaining Useful Life |
| GET | /history | Prediction History |
| GET | /alerts | Active Alerts |
| GET | /health | Component Health |
| GET | /visualizations | SHAP Graphs |
| WS | /ws/simulate | Real-Time Telemetry |

---

# 📈 Results

✅ RMSE: **19.06**

✅ MAE: **14.27**

✅ R² Score: **0.7445**

✅ CPU Inference <100 ms

✅ Explainable Predictions

✅ Real-Time Dashboard

✅ Cloud Deployment

---

# 🌎 Applications

- Aircraft Maintenance
- Aerospace Industry
- Airlines
- Military Aviation
- Industrial Predictive Maintenance
- Wind Turbines
- Marine Engines
- Heavy Machinery
- Manufacturing Plants

---

# 🚀 Future Enhancements

- Transformer Models
- LSTM Prediction
- Mobile Application
- IoT Integration
- AWS Deployment
- Grafana Monitoring
- Kubernetes
- Email Notifications
- SMS Alerts
- Multi-Engine Fleet Monitoring

---

# 👨‍💻 Team

| Name | Role |
|------|------|
| Adrija Adhikary | Machine Learning |
| Dasika Manidhara Adithya Avadhani | Backend Development |
| **Hitesh Kumar S** | Full Stack Development & AI Integration |
| Keerthi Ragav S K | Frontend Development |

---

# ⭐ Project Highlights

- Explainable AI
- Production Ready
- Cloud Native
- Real-Time Monitoring
- Interactive Dashboard
- AI Chat Assistant
- FastAPI Backend
- React Frontend
- WebSocket Streaming
- Docker Deployment

---

# ⭐ If you found this project useful, don't forget to give it a Star!
````
