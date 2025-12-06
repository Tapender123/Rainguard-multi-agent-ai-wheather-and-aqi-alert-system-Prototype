# Rainguard-multi-agent-ai-wheather-and-aqi-alert-system-Prototype
🌦️ Multi-Agent Weather & AQI Alert System
One-Way Automated Rain + Air Quality Alert Architecture for Farmers & Public Safety

This project is a multi-agent automated alert system that sends two types of alerts to users via WhatsApp:

Rain Alerts (light / moderate / heavy) using OpenWeather API

Air Quality Alerts (AQI) using 5-level AQI classification based on WHO criteria

The system is one-way only. Users cannot talk to the system, but every alert includes a “Check Weather Yourself” link.

The purpose is to:

Protect farmers from rain-related crop loss

Improve air-quality awareness using WHO norms

Deliver automated alerts 24×7

Work privately, safely, and reliably at scale

🚀 Project Vision

Farmers and citizens often don’t get timely rain or AQI alerts.
This system solves that using:

Multi-agent fault-tolerant architecture

Automated WhatsApp alerts

WHO-based AQI classification

Privacy-first data handling

Expandability with Google weather systems (like Google Breeze — public domain info)

Goal: Early warnings to protect crops, assets, and health.

🧠 Multi-Agent System Architecture
1. Core Agent

Calls OpenWeather Weather API + Air Pollution API

Calculates:

Rain intensity

Rain probability

AQI category (based on 5-level WHO scale)

Sends the WhatsApp alert

Includes a “👉 Check Weather Yourself” link

2. Backup Agent

Monitors core agent

Auto-activates if:

Core agent fails

API errors

Network interruptions

Ensures no alert is missed

3. Manager / Control Agent

Controls access

Ensures privacy

Logs errors

Supervises both agents

Prevents any direct user–agent interaction

⏱️ Scheduler

Default frequency → Every 4 hours

Fully adjustable (1 hr / 6 hr / custom)

Ensures 24×7 automated monitoring

🌫️ AQI System (5-Level WHO-Based Classification)

The AQI alert system uses only five levels, as required:

AQI Category	Range	Meaning	Emoji
🟢 Good	0–50	Air quality is safe	
🟡 Moderate	51–100	Acceptable; minor risk for sensitive groups	
🟠 Unhealthy for Sensitive Groups	101–150	Children, elderly, sick people affected	
🔴 Unhealthy	151–200	Everyone may experience health effects	
⚫ Hazardous	201+	Serious health impact; avoid outdoor exposure	

WHO norms and protective health advice are included in every alert message.

🌧️ Rain Alert System

Based on OpenWeather API rain data:

Level	Meaning	Emoji
🟢 Light Rain	No major risk	
🟡 Moderate Rain	Take precautions	
🔴 Heavy Rain	High risk for crops, assets	

Flood prediction is NOT included, because OpenWeather does not provide flood alerts.

🔒 Privacy

No user chat

No personal data sharing

Only phone number + location used

Manager agent enforces all safety rules

Designed for full privacy compliance

🌍 Scalability

With Google-scale weather systems:

The platform can support millions

Highly accurate rain + AQI predictions

Rural-friendly WhatsApp delivery

Governments can add public-safety messages

Cost-effective global rollout

📱 User Experience

Users receive:

Clean, color-coded alerts

Rain severity

AQI severity

Health advice

Real-time weather link

No apps. No learning curve. Works anywhere WhatsApp works.

🏗️ Tech Stack

Python

OpenWeather API

WhatsApp (Twilio or alternatives)

APScheduler / Cron

Multi-agent architecture

🎯 Purpose

This system focuses on saving crops, assets, livestocks and human health/lives by giving timely rain and AQI alerts, especially in rural and developing regions.
