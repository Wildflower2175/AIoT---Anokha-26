
A privacy-preserving, TinyML-based edge AI system that intelligently interprets infant cries and environmental conditions to assist caregivers with timely and context-aware alerts.

PROBLEM STATEMENT

Infants primarily communicate through crying, but identifying the underlying reason—such as hunger, discomfort, or emotional distress—can be challenging for caregivers, especially during night-time, in noisy environments, or when they are not physically present. Existing solutions often rely on cloud-based audio streaming, raising concerns related to privacy, latency, and continuous internet dependency.

PROPOSED SOLUTION

The system uses on-device TinyML to classify infant cries into:

Hunger, Physical Discomfort, Emotional distress.

Environmental context such as temperature, humidity, ambient light, and noise patterns is combined with cry classification to prioritize alerts and reduce false alarms. Alerts are delivered locally and remotely while keeping all audio processing fully on-device.

AI&ML Approach:

Audio Feature Extraction: MFCC

Learning Method: Supervised Learning

Model Optimization: INT8 Quantization

Final Model Size: 13.5 KB

Deployment Target: ESP32

Short time-frame audio monitoring enables early detection of soft or repetitive cries while filtering background noise.

HARDWARE 

ESP32 Microcontroller

Microphone Module

DHT11 (Temperature & Humidity)

LDR (Ambient Light)

LED & Buzzer (Local Alerts)

SIMULATION & TOOLS

Model Training: Google Colab

System Simulation: Wokwi

TinyML inference is validated separately; Wokwi is used to demonstrate system behavior.

KEY FEATURES

On-device TinyML inference

Privacy-first design (no raw audio transmission)

Context-aware alerting

Early distress detection

Dual alerts: Local (LED/Buzzer) & Remote (Bluetooth/Wi-Fi)

Low-power, scalable architecture

Team

TinySense Labs

Amrita Vishwa Vidyapeetham
