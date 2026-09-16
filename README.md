# Wound-Wise
Post-Cesarean Early Infection & Sepsis Warning System
A low-cost, non-invasive wearable monitoring system designed to help identify concerning changes during post-cesarean recovery through continuous monitoring of wound and physiological parameters.

Note: This is a prototype early-warning system, not a medical diagnostic device. It does not independently diagnose infection or sepsis.

Problem
Post-cesarean wound infections can initially appear as subtle changes such as:

Increased wound temperature

Redness and swelling

Increasing pain

Abnormal wound discharge

Fever

Changes in heart rate

If these changes are not recognized early, severe infections can potentially progress to complications such as tissue damage and sepsis.

Current post-operative monitoring may involve periodic check-ups, making continuous monitoring outside clinical settings challenging.

Our Solution
We propose a wearable belt that continuously monitors multiple parameters and identifies abnormal trends.

Monitoring Parameters
Parameter	Purpose
🌡️ Body Temperature	Monitors systemic temperature changes
🌡️ Wound Temperature	Monitors local temperature changes around the incision
❤️ Heart Rate	Tracks physiological changes
🫁 SpO₂	Monitors oxygen saturation
📏 Wound-Area Changes	Monitors changes around the wound region
📈 Trend Analysis	Identifies persistent/worsening changes

How It Works

        Sensors
           ↓
    ┌──────────────┐
    │     ESP32     │
    └──────┬───────┘
           ↓
    Data Processing
           ↓
     Trend Analysis
           ↓
   Risk Classification
           ↓
 ┌────────┬────────┬────────┐
 ↓        ↓        ↓
GREEN   YELLOW     RED
Normal  Warning   High Risk
           ↓
     Alert / Action
Risk-Level Concept
🟢 GREEN — Normal
No concerning trend detected.

🟡 YELLOW — Warning
An abnormal or worsening trend has been detected. Continued monitoring and attention are required.

🔴 RED — High Risk
Multiple or persistent concerning changes are detected. The user should seek urgent medical evaluation.

The system does not classify a patient as infected based on a single sensor reading.

Hardware Components
ESP32 Microcontroller

MAX30102 Heart Rate & SpO₂ Sensor

Temperature Sensor(s)

Wound-area sensing mechanism

LEDs

Buzzer

OLED/LCD Display (optional depending on prototype configuration)

Rechargeable Battery / Power Supply

Wearable abdominal belt

Connecting wires and supporting components

Prototype Design
The system is designed as an adjustable abdominal wearable belt.

The belt provides a dedicated area positioned around the C-section wound region for sensing, while physiological sensors can be integrated into the wearable system.

Design Goals
Non-invasive

Lightweight

Comfortable

Portable

Low-cost

Easy to operate

Suitable for continuous monitoring

Key Features
Continuous monitoring

Multi-parameter sensing

Wound-area monitoring

Trend-based risk detection

Green/Yellow/Red alerts

Audible and visual warnings

ESP32-based processing

Potential Wi-Fi/Bluetooth connectivity

Low-cost hardware approach

Innovation
Unlike a conventional thermometer or pulse monitor, our concept combines local wound monitoring and physiological monitoring in a single wearable system.

The main focus is on detecting changes over time rather than relying on one isolated measurement.


Wound Monitoring
       +
Vital Sign Monitoring
       +
Trend Analysis
       ↓
Early Warning
Use Case
The proposed system is intended for women recovering after cesarean delivery.

A possible workflow:


C-Section Recovery
        ↓
Wear Monitoring Belt
        ↓
Continuous Monitoring
        ↓
Abnormal Trend?
     ↙️       ↘️
   NO         YES
   ↓           ↓
GREEN     YELLOW/RED
             ↓
       Medical Evaluation
Future Scope
Future versions could include:

📱 Mobile application

☁️ Cloud-based monitoring

👩‍⚕️ Doctor/caregiver dashboard

📊 Long-term health trend visualization

🤖 AI/ML-based personalized trend analysis

📷 Computer-vision-based wound monitoring

🔋 Improved battery management

🩹 Flexible wearable sensors

🏥 Integration with hospital monitoring systems

🧪 Clinical validation with healthcare professionals

Safety & Limitations
This project is currently a prototype.

Important limitations include:

Sensor readings can be affected by movement and placement.

Environmental conditions can affect temperature measurements.

Wound-area sensing requires further validation.

Risk thresholds require clinical research and validation.

The system cannot independently diagnose infection or sepsis.

Any warning should be evaluated by a qualified healthcare professional.

Project Status
Current Stage: Prototype / Proof of Concept

Completed / Planned
 Wearable belt concept

 ESP32-based architecture

 Multi-parameter monitoring concept

 Risk-level classification concept

 Prototype hardware integration

 Complete wearable packaging

 Mobile application

 Cloud dashboard

 Clinical validation

Technologies
Hardware

ESP32

MAX30102

Temperature sensors

Wound-area sensor

LEDs

Buzzer

Software

Arduino IDE

Embedded C/C++

Sensor data processing

Trend analysis

Team
Project: Post-Cesarean Early Infection & Sepsis Warning System

Developed by:

[S R Adhwitha ]

[Jayasree S K]

[Kavilaya G]

[Ranjana S]

[S P Yogambika ]

Institution: VIT Chennai

Disclaimer
This project is developed for educational, research, and prototype purposes. It is not intended to replace professional medical diagnosis, treatment, or monitoring. The system's measurements and alerts require appropriate technical and clinical validation before any real-world medical use.

⭐ Project Vision
Monitor early. Detect changes. Alert sooner. Support better care.

Early detection can make a difference.

