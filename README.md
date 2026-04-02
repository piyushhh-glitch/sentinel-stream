# sentinel-stream
Real-time fraud detection and decision system using ML + Reinforcement Learning
# 🚀 Sentinel Stream

> Real-time fraud detection and decision intelligence system powered by Machine Learning and Reinforcement Learning.

---

## 🧠 Overview

**Sentinel Stream** is a production-grade, event-driven system designed to detect and prevent financial fraud in real time.

Unlike traditional rule-based systems, it combines:

* **Machine Learning (ML)** → Risk scoring
* **Reinforcement Learning (RL)** → Adaptive decision making
* **Streaming Architecture** → Low-latency processing (<50ms)

---

## ⚡ Key Features

* 🔍 Real-time fraud detection
* 🧠 Behavioral anomaly detection (Isolation Forest)
* 🤖 RL-based decision engine (Approve / Block / OTP)
* ⚡ Sub-50ms decision latency
* 📡 Event-driven architecture using Kafka
* 🧱 Stateful feature store using Redis
* 📊 Live monitoring with Grafana
* 🐳 Fully containerized with Docker

---

## 🏗️ System Architecture

```
Client → FastAPI → Redis (Feature Store)
                  ↓
             ML Model (Risk Score)
                  ↓
            RL Agent (Decision)
                  ↓
      Kafka → PostgreSQL + Monitoring
```

---

## 🧰 Tech Stack

| Layer         | Technology            |
| ------------- | --------------------- |
| API           | FastAPI               |
| Feature Store | Redis                 |
| Streaming     | Kafka                 |
| ML            | Scikit-learn, XGBoost |
| RL            | Q-Learning / DQN      |
| Database      | PostgreSQL            |
| Dashboard     | Streamlit             |
| Monitoring    | Prometheus + Grafana  |
| Deployment    | Docker                |

---

## 📁 Project Structure

```
sentinel-stream/
│
├── api/              # FastAPI application
├── simulator/        # Transaction generator (Faker)
├── models/           # ML models
├── rl_agent/         # Reinforcement learning agent
├── feature_store/    # Redis integration
├── kafka/            # Producers and consumers
├── dashboard/        # Streamlit dashboard
├── infra/            # Docker & infra configs
├── configs/          # Config files
├── tests/            # Unit tests
│
├── README.md
├── requirements.txt
└── docker-compose.yml
```

---

## 🔄 Execution Flow

1. Transaction received via FastAPI
2. Features enriched using Redis
3. ML model generates risk score
4. RL agent selects optimal action
5. Decision returned (Approve / Block / OTP)
6. Transaction streamed to Kafka
7. Stored in PostgreSQL + monitored

---

## 🎯 Goal

To build a **scalable, intelligent fraud detection system** that balances:

* Fraud prevention 💸
* User experience 😊

---

## 🚀 Getting Started (Coming Soon)

---

## 📌 Author

Built as part of a real-world ML + Systems Engineering project.
