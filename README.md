# ARGUS
### Automated Risk & Guard Unified System

ARGUS is a real-time industrial IoT monitoring system that tracks machine health using sensors, processes data through a Python backend, and visualizes insights in a React dashboard.

It simulates predictive maintenance systems used in modern industrial environments.

---

## Overview

ARGUS collects sensor data (temperature, vibration, load), processes it into meaningful metrics, and displays machine health scores, risk level classification, real-time alerts, and predictive maintenance insights.

The system is designed to evolve into a full industrial monitoring platform with IoT, AI, and cloud integration.

---

## Features

- Real-time sensor monitoring (simulated or hardware-based)
- Machine health scoring system
- Risk detection (Normal / Warning / Critical)
- Live alert system
- Sensor data visualization (charts and graphs)
- Predictive maintenance recommendations (planned)
- Responsive React dashboard UI
- Light and dark mode (planned)

---

## System Architecture

ESP32 / Arduino Sensors → Python Processing Engine → API Layer (FastAPI / Flask - planned) → React Dashboard UI

---

## Tech Stack

Frontend:
- React (Vite)
- JavaScript
- Recharts (visualizations)
- Framer Motion (animations)
- React Icons
- CSS Variables System

Backend (Planned / In Progress):
- Python
- FastAPI or Flask
- Pandas and NumPy

Hardware (Optional / Future):
- ESP32 / Arduino
- Temperature sensor
- Vibration sensor
- Potentiometer (load simulation)

---

## Demo Mode

ARGUS currently runs in simulation mode. Sensor data is randomly generated or mocked. No physical hardware is required. Backend APIs are optional at this stage. This allows full frontend development without hardware dependency.

---

## Environment Variables Setup

ARGUS uses environment variables for secure configuration.

Create a `.env` file in the root directory:

```env
VITE_API_KEY=your_api_key_here
VITE_API_BASE_URL=http://localhost:5000
```

Important:
- Never commit `.env` files
- `.env` is included in `.gitignore`
- Each user must create their own API keys

---

## API Integration (Future)

When backend is enabled, ARGUS will connect to a Python API.

Example workflow:
1. Sensor data is sent to backend
2. Python processes and calculates health score, risk level, and failure probability
3. React dashboard fetches processed data

Example endpoints:
GET /api/sensors
GET /api/health
GET /api/risk
POST /api/data

---

## Getting Started

### Clone repository
git clone https://github.com/amorsaralynn08-arch/ARGUS.git
cd ARGUS

### Install dependencies
npm install

If needed:
npm install react-icons recharts framer-motion react-router-dom

### Start development server
npm run dev

### Open in browser
http://localhost:5173

---

## Project Structure

src/
├── components/
├── pages/
├── data/
├── styles/
├── context/
├── utils/
├── App.jsx
└── main.jsx

---

## Future Improvements

- Machine learning failure prediction
- Real-time database integration (Firebase or PostgreSQL)
- MQTT live sensor streaming
- Cloud deployment dashboard
- Mobile version
- Real hardware integration (ESP32)
- Advanced analytics engine

---

## Author

Amor

---

## License

This project is licensed under the MIT License.