# Nova SIEM — Real-Time Threat Detection System

## Overview

A real-time Security Information and Event Management (SIEM) system designed to detect, analyze, and respond to security threats using centralized logging and automated alerting.

## Problem Statement

Traditional systems detect threats too late or require manual monitoring. This project simulates a real-world SIEM pipeline to enable proactive threat detection.

## Architecture

Logs → Logstash → Elasticsearch → Kibana → Alert Engine

## Features

* Real-time log ingestion
* Threat detection (e.g., brute force, failed logins)
* Alert generation
* Dashboard visualization
* Incident simulation

## Tech Stack

* Elasticsearch
* Logstash
* Kibana
* Python (Flask)
* Docker (optional)

## Project Structure

```bash
backend/       # Application logic
configs/       # ELK configurations
docs/          # Documentation
data/          # Sample logs
```

## Setup Instructions

### 1. Clone Repo

```bash
git clone https://github.com/yourusername/nova-siem.git
cd nova-siem
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run Services

```bash
python backend/app.py
```

### 4. Access Dashboard

* Kibana → http://localhost:5601

## Detection Scenarios

* Multiple failed login attempts
* Suspicious IP activity
* Log anomalies

## Results

* Reduced detection latency from minutes → seconds
* Real-time alert generation validated with simulated attacks

## Future Improvements

* ML-based anomaly detection
* Integration with cloud SIEM tools
* Automated incident response

## Author

devbadri13
