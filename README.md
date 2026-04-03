# Monitoring & Alerting System (DevOps Project)

## Overview
This project demonstrates a complete **end-to-end monitoring and alerting system** using Prometheus, Grafana, and Docker.

It includes both:
- **Infrastructure monitoring** (CPU, memory)
- **Application-level monitoring** (Flask app metrics)

The system not only visualizes data but also **detects issues and sends alerts via email**, simulating real-world DevOps workflows.

---

## Tech Stack
- Docker & Docker Compose  
- Prometheus  
- Grafana  
- Node Exporter  
- Flask (Python)  

---

## Features

### Infrastructure Monitoring
- CPU and memory usage tracking using Node Exporter  
- Real-time dashboards built in Grafana  

---

### Application Monitoring
- Flask application exposing Prometheus metrics (`/metrics`)  
- Custom metric: `app_requests_total`  
- Requests per second (RPS) visualization  

---

### Alerting System
- High CPU usage alert  
- No traffic alert (detects inactivity)  
- High traffic alert (detects spikes)  

---

### Notifications
- Email alerts configured using Grafana SMTP  
- Thresholds and timing adjusted to avoid alert fatigue  

---

## How to Run

```bash
docker-compose up -d --build
```
## 🧠 Key Learnings
- Difference between monitoring and observability
- Writing Prometheus queries for real metrics
- Alert tuning (thresholds, evaluation time, stability)
- Debugging Docker volumes and persistence issues
- Handling real-world issues like alert fatigue
