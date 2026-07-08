# Smart Crowd Monitoring & Network Intelligence System

An AI-powered smart crowd monitoring platform that combines **Computer Vision**, **Machine Learning**, and a **Spring Boot backend** to monitor crowd density, generate real-time alerts, analyze network connectivity, and visualize live analytics through an interactive dashboard.

The system processes CCTV video streams using **YOLOv8**, estimates crowd density, generates heatmaps, integrates WiFi probe data, and exposes processed insights through REST APIs and WebSockets for real-time visualization.

---

## 🚀 Key Features

### 🤖 AI & Machine Learning (Core Module)

The AI engine performs real-time crowd analysis from CCTV feeds using computer vision.

### Features

- Real-time people detection using **YOLOv8**
- Crowd counting from video streams
- Crowd density estimation
- Heatmap generation for crowded regions
- Evacuation path analysis
- WiFi probe integration for device estimation
- Zone-wise analytics generation
- Live statistical analysis
- AI REST API for backend integration

The AI module converts raw CCTV footage into meaningful analytics that can be consumed by the backend.

---

### ☕ Spring Boot Backend

The backend acts as the central processing layer between AI services and the dashboard.

### Responsibilities

- Receives AI-generated crowd analytics
- Processes zone-wise statistics
- Calculates:
  - Crowd Density
  - Risk Score
  - Entry Rate
  - Exit Rate
  - Network Score
- Stores historical analytics in MongoDB
- Generates crowd alerts
- Provides REST APIs
- Broadcasts live updates using WebSockets

---

### 💻 Frontend

A lightweight dashboard built to visualize the processed analytics.

Features include:

- Live crowd monitoring
- Zone-wise statistics
- Heatmap visualization
- Alert notifications
- Historical trend charts

The frontend primarily serves as a visualization layer while most of the intelligence resides in the AI and backend modules.

---

# 🏗️ System Architecture

```
                CCTV Camera
                     │
                     ▼
          AI/ML (YOLOv8 Detection)
                     │
     Crowd Count • Heatmap • Analytics
                     │
          FastAPI / Python APIs
                     │
                     ▼
        Spring Boot Backend
                     │
     Risk Analysis • Alerts • MongoDB
                     │
         REST APIs & WebSockets
                     │
                     ▼
        React Dashboard (Frontend)
```

---

# 🧠 AI/ML Technologies

- Python
- YOLOv8
- OpenCV
- NumPy
- FastAPI
- Computer Vision
- Heatmap Generation
- Crowd Density Analysis

### AI Modules

```
crowd/
│
├── api.py
├── main.py
├── model.py
├── crowd_analysis.py
├── heatmap.py
├── evacuation.py
├── wifi_probe.py
├── stats.py
├── cctv_stream.py
└── db.py
```

---

# ☕ Backend Technologies

- Java
- Spring Boot
- Spring Web
- Spring Data MongoDB
- MongoDB Atlas
- Spring WebSocket
- Maven

### Backend Modules

```
backend/
│
├── controller
├── service
├── repository
├── model
├── dto
├── websocket
└── config
```

---

# 💻 Frontend Technologies

- React
- TypeScript
- Vite
- Tailwind CSS

---

# 📊 AI Processing Workflow

1. Capture CCTV video stream
2. Detect people using YOLOv8
3. Count people in each zone
4. Generate crowd density
5. Create heatmaps
6. Analyze WiFi probe data
7. Send processed analytics to Spring Boot backend
8. Backend stores data in MongoDB
9. Dashboard receives live updates via WebSockets

---

# 📈 Analytics Generated

- Total Crowd
- Crowd Density
- Crowd Intensity
- Risk Score
- Entry Rate
- Exit Rate
- Network Score
- Heatmaps
- Zone Analytics
- Historical Trends

---

# 🛠️ Tech Stack

| Layer | Technology |
|--------|------------|
| AI/ML | Python, YOLOv8, OpenCV, NumPy, FastAPI |
| Backend | Java, Spring Boot, MongoDB, WebSocket |
| Frontend | React, TypeScript, Tailwind CSS |
| Database | MongoDB Atlas |

---

# 📂 Project Structure

```
Smart Crowd Monitoring
│
├── crowd/          # AI & Machine Learning
├── backend/        # Spring Boot Backend
└── frontend/       # React Dashboard
```

---

# ⭐ Future Enhancements

- Predictive crowd forecasting
- Multi-camera tracking
- Face anonymization for privacy
- Edge deployment using Raspberry Pi
- LoRa/WiFi HaLow integration
- Mobile dashboard
- AI-based emergency evacuation recommendations

---

# 👩‍💻 Author

**Nidhi Sharma**

Backend & AI/ML Developer

- Spring Boot
- Java
- Python
- Computer Vision
- Machine Learning
- MongoDB
