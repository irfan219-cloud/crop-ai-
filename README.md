AI & IoT-Powered Smart Agriculture Platform for Pest Control, Crop Monitoring, and Market Intelligence

📌 Problem Statement

Farmers face devastating crop losses—often up to 40% pre-harvest—due to invisible threats they cannot easily detect. These include:

Subsurface soil moisture imbalance

Sudden temperature and humidity changes

Rapidly spreading pests like Fall Armyworm

Delayed access to real-time market price trends

My family has personally suffered these losses.
Between 2022–2024, pest attacks severely damaged our legume farms, leading to major financial setbacks and nearly costing my brother an extra year in school.
In November 2025, our cocoa farm recorded heavy losses simply because we lacked real-time market price intelligence.

These experiences inspired CropGuard — a platform designed to protect farmers before losses occur, not after.

🚀 Solution Overview

CropGuard is a smart agriculture web application that combines:

IoT-based subsurface farm monitoring

AI-powered pest detection

Weather forecasting

Market trend intelligence

Personal AI farm advisor

SMS alerts and expert directory

It empowers farmers with real-time insights, early warnings, and actionable recommendations.

🧠 What CropGuard Does
1️⃣ Subsurface Environment Monitoring (IoT + Wokwi)

Monitors:

🌡 Temperature

💧 Humidity

🌱 Soil Moisture

☀️ Light Intensity

Uses simulated sensors:

DHT22

Soil Moisture Sensor

LDR

ESP32 microcontroller displays live data on a 20x4 LCD

Sends SMS alerts when conditions become critical

Provides AI-powered recommendations via Farm Advisor

2️⃣ Weather Forecast Intelligence (Open-Meteo API)

Location-based multi-day forecasts:

Temperature

Humidity

Rainfall probability

Enables:

Smart irrigation scheduling

Harvest planning

Risk mitigation against extreme weather

3️⃣ AI Pest Detection (Machine Learning)

Farmers upload crop images via mobile

AI model detects pests like:

🐛 Fall Armyworm

Provides:

Pest identification

Targeted control strategies

Prevention recommendations

4️⃣ Farm Advisor & Market Intelligence

AI Farm Advisor:

Monitors farm status when the farmer is offline

Gives actionable insights

Market trend alerts:

Notifies farmers of price drops or spikes

Expert Directory:

Connects farmers to nearby agronomists and agri-input stores

🏗️ How It Was Built
🔌 Hardware Simulation (IoT)

Platform: Wokwi

Microcontroller: ESP32 Dev Kit

Sensors:

DHT22 (Temperature & Humidity)

LDR (Light)

Soil Moisture Sensor

Live values simulated via sliders

💻 Embedded Software

Language: C++ (Arduino)

GPIO Pins:

GPIO 2 – DHT22

GPIO 36 – Soil Moisture

GPIO 34 – LDR

Libraries Used:

LiquidCrystal_I2C

Displays real-time data on 20x4 LCD

📊 Data Processing

Raw sensor values converted into:

Calibrated moisture percentage (0–100%)

Temperature (°C)

Light intensity (Lux)

🤖 AI Framework

Pest Detection Model:

Hosted on Hugging Face

Integrated into web app

Cloud logic designed for:

Predictive modeling

Image processing

Future analytics expansion

🌐 Web App

Built using lovable.dev

Unified dashboard showing:

Sensor data

Weather forecast

Pest detection results

Market insights

Integrated:

AI Assistant

SMS notifications (Twilio – limited by free tier)

⚠️ Challenges Faced

Hosting live ML model endpoints

Filtering noisy datasets during transfer learning

Free-tier limitations of Twilio SMS

Poor initial pest detection accuracy in video inputs

Sensor value calibration on Wokwi

Resource limits on lovable.dev

Hardware constraints for real-world deployment

🏆 Accomplishments

✅ Fully simulated end-to-end IoT system

✅ Live sensor-to-LCD and sensor-to-web synchronization

✅ AI-powered pest detection workflow

✅ Farm Advisor that works even when the farmer is offline

✅ Clean, simplified dashboard for farmers

✅ Clear technical solution to Fall Armyworm infestation

✅ Strong business model insights

✅ High scalability potential across Africa and developing regions

✅ Clear employment creation pathway

📚 What I Learned

IoT integration with cloud platforms

Hosting ML models on Hugging Face

Weather API integration (Open-Meteo)

Real-world calibration of sensor data

AI + IoT system architecture

Product thinking for farmers, not just tech demos

🔮 What’s Next for CropGuard

Planned future enhancements (detailed on Slide 24):

Physical hardware deployment on real farms

Advanced pest video detection with auto-zoom

Blockchain-based produce traceability

Market price prediction using time-series models

Government & NGO integration

Multilingual voice assistant for farmers
