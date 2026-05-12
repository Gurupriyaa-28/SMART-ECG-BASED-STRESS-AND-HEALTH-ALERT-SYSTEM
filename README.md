💓 Smart ECG-Based Stress & Health Alert System

A compact real-time biomedical monitoring system designed to observe ECG activity, measure heart rate, analyze stress levels, and send emergency alerts using GSM technology.

📌 Introduction

The Smart ECG-Based Stress & Health Alert System is built using the AD8232 ECG sensor and Arduino Uno to continuously monitor cardiac activity. The system captures ECG signals from the body, processes them to determine BPM (Beats Per Minute), evaluates stress conditions, and generates alerts through LEDs, OLED display, and GSM communication.

This project provides an affordable and efficient solution for preventive healthcare and remote patient monitoring.
🧠 Technologies & Concepts

The project combines biomedical signal processing with embedded system design using concepts such as:

Electrocardiography (ECG)
Analog signal acquisition
Moving average filtering
R-peak detection
BPM estimation using peak intervals
GSM-based communication
Real-time embedded programming
🧩 Components Required
| Component              | Purpose                       |
| ---------------------- | ----------------------------- |
| Arduino Uno            | Main controller               |
| AD8232 ECG Module      | ECG signal acquisition        |
| ECG Electrodes         | Detect heart signals          |
| OLED Display (SSD1306) | Display BPM and stress status |
| GSM Module (SIM800L)   | Send SMS alerts               |
| LEDs                   | Stress indication             |
| Battery / USB Supply   | Power source                  |
🔌 Circuit Connections
| Module     | Arduino Pin |
| ---------- | ----------- |
| AD8232 OUT | A0          |
| LO+        | D10         |
| LO-        | D11         |
| OLED SDA   | A4          |
| OLED SCL   | A5          |
| GSM TX     | D7          |
| GSM RX     | D8          |
| LEDs       | D4, D5, D6  |
⚙️ System Operation
ECG electrodes collect heart signals from the body.
The AD8232 module amplifies and conditions the ECG waveform.
Arduino reads the analog ECG signal.
A moving average filter smooths the waveform.
R-peaks are detected using threshold comparison.
BPM is calculated from the interval between peaks.
Stress level is identified based on BPM values:
Below 60 BPM → Low
60–100 BPM → Medium
Above 100 BPM → High
Results are shown on the OLED display.
LEDs visually indicate stress condition.
GSM module sends SMS alerts during abnormal conditions.
💻 Software Details
Development Platform: Arduino IDE
Programming Language: Embedded C/C++
Libraries Used:
Adafruit SSD1306
Adafruit GFX
SoftwareSerial
🚨 Stress Alert Conditions
| BPM Range  | Stress Level | Indication    |
| ---------- | ------------ | ------------- |
| < 60 BPM   | Low          | Green LED     |
| 60–100 BPM | Medium       | Yellow LED    |
| > 100 BPM  | High         | Red LED + SMS |
🛠️ Knowledge & Skills Acquired
Embedded systems design
ECG signal analysis
Sensor interfacing
GSM communication
Arduino programming
Real-time monitoring
Hardware debugging

🌍 Practical Applications
Personal healthcare systems
Stress monitoring devices
Remote patient observation
Early cardiac abnormality detection
Wearable biomedical devices

⚠️ Existing Limitations
ECG noise caused by body movement
Dependence on correct electrode placement
Simple BPM-based stress analysis
GSM module power fluctuations

🔮 Future Improvements
IoT/cloud monitoring integration
Mobile application support
AI-driven stress prediction
Compact wearable implementation
Advanced ECG filtering algorithms

👩‍💻 Team
Kesihambigai
Gurupriyaa

📚 References
Arduino Documentation
AD8232 Datasheet by Analog Devices
IEEE Research Papers on ECG Monitoring





