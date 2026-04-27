# Solar Microgrid Cyberattack Detection System

A machine learning-based intrusion detection system (IDS) for solar microgrid infrastructure, 
developed as a capstone project for Pinellas County, Florida. The system detects six classes 
of cyberattacks on photovoltaic (PV) energy systems using a feedforward neural network 
achieving 96.23% classification accuracy.

---

##  Demo
> ## 📽️ Demo
[![Demo Video](https://img.shields.io/badge/Watch-Demo-red?logo=youtube)](https://youtu.be/pjCUcDkSabk)
> 

---

##  Project Overview

Critical infrastructure such as solar microgrids is increasingly vulnerable to cyberattacks 
that can disrupt energy generation, damage equipment, and destabilize the grid. This project 
addresses that threat by building an AI-powered detection system trained on simulated attack 
data from two real Pinellas County solar sites.

**Location:** Pinellas County, Florida  
**Sites:** Market Parking Lot PV System, Public Park PV System  
**Simulation Tool:** HelioScope  
**Academic Institution:** James Madison University — ISAT 490 Capstone

---

## Attack Classes Detected

The model classifies normal operation and six cyberattack scenarios:

| Class | Attack Type |
|-------|-------------|
| 0 | Normal Operation |
| 1 | False Data Injection |
| 2 | Inverter Manipulation |
| 3 | Output Drop |
| 4 | Sensor Spoofing |
| 5 | Clipping Attack |


---

##  Model Performance

| Metric | Score |
|--------|-------|
| Accuracy | **96.23%** |
| Architecture | Feedforward Neural Network |
| Framework | TensorFlow / Keras |
| Training Data | HelioScope simulation + synthetic attack injection |

---

##  System Architecture
HelioScope Simulation Data
↓
Synthetic Attack Injection
↓
Feature Engineering + Preprocessing
↓
Feedforward Neural Network (TensorFlow/Keras)
↓
Flask Operator Dashboard
├── Role-Based Authentication
├── Real-Time Risk Scoring
├── Chart.js Visualizations
└── Attack Classification Display
---

##  Tech Stack

| Component | Technology |
|-----------|------------|
| Machine Learning | Python, TensorFlow, Keras |
| Web Framework | Flask |
| Visualizations | Chart.js |
| Authentication | Role-based access control (RBAC) |
| Data Simulation | HelioScope, HOMER Pro |
| Data Processing | Pandas, NumPy, Scikit-learn |

------

##  Running the Project

### Prerequisites
```bash
pip install -r requirements.txt
```

### Run the Flask Dashboard
```bash
python app.py
```

Navigate to `http://localhost:5000` in your browser.

### Run in Google Colab
Open `UpdatedCapstone_3_2.ipynb` in Google Colab and run all cells.  

------

##  Security & Compliance

This project incorporates relevant regulatory standards for solar energy systems:

- **NEC Articles** — National Electrical Code compliance for PV systems
- **Florida Statutes** — State-level energy infrastructure regulations
- **ICS/OT Security** — Industrial Control System threat modeling

