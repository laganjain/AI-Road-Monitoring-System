# 🚧 AI Road Monitoring & Incident Response System
### Team: Wall Breakers (Lagan Jain & Palak Shukla)  
National Road Safety Hackathon 2025 – CoERS, IIT Madras

## 🌍 Overview
This project is a real-time road hazard reporting and detection platform that combines:

1. Crowdsourced user reports (potholes, waterlogging, accidents, traffic, road closure)
2. IoT sensor-based automatic detection (via ESP32 + sensors)
3. Live dashboard powered by Firebase Firestore

It is designed especially for Tier 2/3 India under the theme **Build for Bharat**.

## 🎯 Features
- Real-time hazard reporting web app
- Sensor + manual reporting fusion
- Live dashboard (no refresh needed)
- Firebase Authentication (login, sign up, reset password)
- Newest hazards shown first
- Lightweight UI suitable for low-bandwidth environments

## 🛠 Tech Stack
- HTML, CSS, JavaScript
- Firebase Authentication
- Firebase Firestore (Realtime)
- (Optional) Firebase Hosting
- IoT: ESP32, MPU-6050, GPS, Ultrasonic, OBD-II (concept demo)

## 🗄 Firestore Collection: `road_reports`
Each document contains fields like:
- `type` (string)
- `locationName` (string)
- `userEmail` (string)
- `userId` (string)
- `timestamp` (timestamp)
- `source` ("manual" / "sensor")
- `sensorData` (object with vibration, waterLevel, etc.)

## 🚀 How to Run Locally
1. Clone/download this repo.
2. Create a Firebase project, enable **Auth (Email/Password)** and **Firestore**.
3. Replace values in `firebaseConfig.js` with your Firebase config.
4. Open `index.html` using a local server (VS Code Live Server recommended).
5. Sign up, log in, and start submitting demo reports.

## 👥 Team
- **Lagan Jain** – Full Stack + Firebase + Sensors
- **Palak Shukla** – UX, flows, documentation

## 📝 License
MIT License
