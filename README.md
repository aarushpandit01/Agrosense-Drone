<div align="center">

#  AgroSense

### *AI-Powered Precision Agriculture Drone*


*"Empowering Farmers Through Edge AI and Autonomous Robotics"*

---

![Status](https://img.shields.io/badge/Status-In%20Development-orange)
![Platform](https://img.shields.io/badge/Platform-ESP32%20%7C%20Raspberry%20Pi-blue)
![Language](https://img.shields.io/badge/Language-C%2B%2B%20%7C%20Python-success)
![License](https://img.shields.io/badge/License-MIT-green)

</div>

---

# Overview

AgroSense is a next-generation precision agriculture platform that combines **embedded systems**, **computer vision**, and **edge AI** to assist farmers with intelligent crop monitoring.

The system is split into two independent subsystems:

**Flight Control** — ESP32 + F722

**Vision AI** — ESP32-CAM + Raspberry Pi

Together they enable autonomous data collection and real-time crop analysis.

---

# Features

-  Intelligent Flight Control
-  Live Wi-Fi Video Streaming
-  GPS Navigation
-  Edge AI Processing
-  Crop Disease Detection
-  Modular Embedded Architecture

---

# System Architecture

```mermaid
flowchart LR

subgraph Flight_System
GPS[🛰 GPS Module]
ESP32[⚡ ESP32 Controller]
F722[🎮 F722 Flight Controller]
ESC[⚙️ ESCs]
MOTORS[🚁 BLDC Motors]

GPS --> ESP32
ESP32 -->|UART / MSP| F722
F722 --> ESC
ESC --> MOTORS
end

subgraph Vision_System
CAM[📷 ESP32-CAM]
PI[🍓 Raspberry Pi 4]
AI[🧠 AI Engine]
DISEASE[🌱 Disease Detection]
DASH[📊 Dashboard]

CAM -->|Wi-Fi| PI
PI --> AI
AI --> DISEASE
DISEASE --> DASH
end
```

---

# 🛠 Hardware

| Component | Purpose |
|-----------|---------|
| ESP32 | Drone Controller |
| F722 FC | Flight Stabilization |
| ESP32-CAM | Live Video |
| Raspberry Pi 4 | Edge AI |
| GPS | Navigation |
| ESCs | Motor Control |
| BLDC Motors | Flight |
| LiPo Battery | Power |

---

# 💻 Software Stack

| Embedded | AI | Tools |
|----------|----|-------|
| C++ | OpenCV | Arduino IDE |
| Arduino | TensorFlow / YOLO *(Planned)* | Git |
| UART | Python | VS Code |

---


---

# 📈 Development Roadmap

- [x] Hardware Selection
- [x] Drone Assembly
- [x] ESP32 ↔ F722 Communication
- [x] ESP32-CAM Streaming
- [ ] Raspberry Pi AI Integration
- [ ] Disease Detection Model
- [ ] Autonomous Navigation
- [ ] Field Testing

---

# Vision
Our goal is to build an affordable autonomous drone capable of assisting farmers through **AI-powered crop monitoring**, reducing manual inspection time and enabling data-driven agricultural decisions.

---

<div align="center">

### Built with passion by **ArcNexus Labs**

*"Engineering Tomorrow's Agriculture."*

</div>
