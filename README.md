# FALCON
AI-powered agricultural drone built using ESP32, GPS, and embedded systems for precision farming.
## -System Architecture

```mermaid
flowchart LR

    GPS[GPS Module]
    ESP32[ESP32 Flight Controller]
    ESC[Electronic Speed Controllers]
    MOTOR[BLDC Motors]

    CAM[ESP32-CAM]
    PI[Raspberry Pi 4]
    AI[AI Inference]
    DISEASE[Crop Disease Detection]
    DASH[Farmer Dashboard / Alerts]

    GPS --> ESP32
    ESP32 --> ESC
    ESC --> MOTOR

    CAM -->|Wi-Fi Video Stream| PI
    PI --> AI
    AI --> DISEASE
    DISEASE --> DASH
```
