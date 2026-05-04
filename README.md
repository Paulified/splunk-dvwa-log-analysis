# Splunk DVWA Log Analysis

## 📌 Overview
This project demonstrates how to collect and analyze web server logs using Splunk from a DVWA (Damn Vulnerable Web Application) running in Docker.

## 🎯 Objectives
- Deploy DVWA using Docker
- Generate web traffic (normal and malicious)
- Extract logs from the container
- Upload logs into Splunk
- Analyze logs using Splunk queries

## 🛠 Tools Used
- Kali Linux
- Docker
- Splunk Cloud
- DVWA

## ⚙️ Setup
1. Start DVWA container using Docker
2. Access DVWA via browser (port 8080)
3. Generate traffic (login attempts, injections)
4. Extract logs from container

## 📂 Logs
Logs are stored in the /logs folder.

## 🔍 Splunk Queries

### View all logs
index=main

### Detect SQL Injection
index=main "OR 1=1"

### Detect Command Injection
index=main "whoami"

## 📊 Results
- Successfully ingested logs into Splunk
- Identified suspicious patterns in traffic

## 📸 Screenshots
See /screenshots folder.

## 🧠 Lessons Learned
- Troubleshooting log extraction issues
- Understanding Splunk search basics
- Working with Docker containers

## 🚀 Future Improvements
- Real-time log forwarding
- Splunk dashboards
- Better log parsing