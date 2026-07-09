# FALCON
AI-powered agricultural drone built using ESP32, GPS, and embedded systems for precision farming.

## System Architecture

```mermaid
flowchart TD

%% Flight Control
GPS[GPS Module]
ESP32[ESP32 Controller]
F722[F722 Flight Controller]
ESC[Electronic Speed Controllers]
MOTORS[BLDC Motors]

GPS --> ESP32
ESP32 -->|UART / MSP| F722
F722 --> ESC
ESC --> MOTORS

%% AI Pipeline
CAM[ESP32-CAM]
PI[Raspberry Pi 4]
AI[Computer Vision & AI]
DISEASE[Crop Disease Detection]
ALERTS[Farmer Dashboard / Alerts]

CAM -->|Wi-Fi Video Stream| PI
PI --> AI
AI --> DISEASE
DISEASE --> ALERTS
```
