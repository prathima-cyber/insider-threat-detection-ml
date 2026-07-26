# Insider Threat Detection Using User Behaviour Analytics & Machine Learning

## 📌 Project Overview

Insider threats are cybersecurity risks caused by users who have authorized access to an organization's systems and data. This project uses **User Behaviour Analytics (UBA)** and **Machine Learning** to identify unusual user activity and detect potential insider threats.

The system analyzes simulated user activity logs such as logins, file access, file downloads, email activity, USB usage, and file deletion. Behavioural features are extracted and analyzed to identify abnormal patterns.

## 🎯 Objectives

* Detect unusual user behaviour.
* Identify potential insider threats.
* Build behavioural profiles for users.
* Detect anomalies using machine learning.
* Assign risk levels to suspicious activity.
* Provide visual reports for security analysis.

## 🔄 Project Workflow

```text
User Activity Logs
       ↓
Data Preprocessing
       ↓
Feature Engineering
       ↓
User Behaviour Baseline
       ↓
Isolation Forest
       ↓
Risk Score Calculation
       ↓
Normal / Medium / High Risk
       ↓
Visualization & Alerts
```

## 🛠️ Technologies Used

* **Programming:** Python
* **Data Processing:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Algorithms:** Isolation Forest, Random Forest
* **Visualization:** Matplotlib
* **Development Environment:** Visual Studio Code

## 🔍 Features

### 1. Activity Log Generation

The project generates synthetic user activity logs containing:

* User ID
* Timestamp
* Event type
* Data transferred
* Activity label

### 2. Behavioural Feature Engineering

The system calculates features such as:

* Total events
* Unique event types
* Total data transferred
* Maximum data transferred
* Off-hours activity
* Risky event count
* Behaviour deviation from the user's baseline

### 3. Anomaly Detection

**Isolation Forest** is used to detect unusual behaviour without requiring a predefined threat label.

### 4. Risk Scoring

Each user activity profile receives a risk score from **0–100** and is classified as:

* 🟢 Normal
* 🟡 Medium
* 🔴 High

### 5. Machine Learning Comparison

A **Random Forest classifier** is also used with the synthetic labels to compare supervised classification performance.

### 6. Visualization

The project generates charts showing:

* User risk distribution
* Top risky user profiles
* Important behavioural features

## 📂 Project Structure

```text
insider-threat-detection/
│
├── data/
│   └── README.md
│
├── outputs/
│   └── README.md
│
├── src/
│   └── main.py
│
├── .gitignore
├── README.md
└── requirements.txt
```

## ▶️ How to Run

### Step 1: Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd insider-threat-detection
```

### Step 2: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 3: Run the project

```bash
python src/main.py
```

### Step 4: Check results

After execution, generated reports and visualizations will be available inside:

```text
outputs/
```

## 📊 Output

The project generates:

* `user_risk_report.csv`
* `high_risk_alerts.csv`
* `risk_distribution.png`
* `top_risk_scores.png`
* `feature_importance.png`

## 🔐 Cybersecurity Application

This project demonstrates how User Behaviour Analytics and machine learning can support proactive detection of suspicious insider activity. It can be further extended to work with enterprise SIEM platforms and real-time security monitoring systems.

## 🚀 Future Enhancements

* Integrate real CERT insider-threat datasets.
* Develop a web dashboard using Streamlit.
* Add LSTM/deep-learning-based sequence analysis.
* Integrate with SIEM platforms such as Splunk or QRadar.
* Add real-time log monitoring and alert notifications.
* Improve privacy and access-control mechanisms.

## ⚠️ Disclaimer

This project uses **synthetic activity data** for academic and demonstration purposes. It should not be used to monitor real users without proper authorization, privacy controls, and applicable compliance requirements.

## 👩‍💻 Author

**G. Prathima**
B.Tech – Computer Science & Engineering (Cyber Security)

**Project:** Insider Threat Detection Using User Behaviour Analytics & Machine Learning
