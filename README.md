# 🛡️ Military Intelligence Dashboard

## 📌 Project Overview

The **Military Intelligence Dashboard** is an AI-powered, data-driven web application designed to analyze global terrorism and security-related incidents through interactive visualizations, machine learning, threat assessment, and forecasting.

The system transforms historical terrorism data into meaningful intelligence insights by providing geographical threat visualization, country-level analysis, attack prediction, threat-level assessment, trend forecasting, and AI-assisted intelligence analysis through an interactive dashboard.

The project is developed using **Python and Streamlit**, with machine learning and data analytics techniques used to support predictive and exploratory intelligence functions.

---

## 🎯 Objectives

The primary objectives of the Military Intelligence Dashboard are to:

* Analyze historical global terrorism and security incident data.
* Visualize geographical distribution and concentration of threats.
* Perform country-level terrorism and security analysis.
* Predict attack-related outcomes using a trained machine learning model.
* Assess and categorize potential threat levels.
* Identify historical patterns and forecast future trends.
* Provide an interactive environment for exploring intelligence data.
* Present complex security information through clear and accessible visualizations.

---

## 🚀 Key Features

### 🌍 Global Threat Map

Provides an interactive geographical representation of terrorism-related incidents, helping users identify regions with higher concentrations of reported incidents.

### 🔍 Country Analysis

Enables detailed analysis of terrorism patterns at the country level, including historical trends and incident characteristics.

### 🎯 Attack Prediction

Uses a trained machine learning model to generate predictions based on selected incident-related features.

### 🚨 Threat Level Assessment

Provides a threat assessment interface for analyzing incident characteristics and determining an appropriate threat category based on the implemented analytical approach.

### 📈 Forecasting

Analyzes historical trends to provide forecasting-oriented insights into terrorism and security incident patterns.

### 🧠 AI Intelligence

Provides an AI-assisted intelligence interface for generating analytical insights from the available security data.

### 📊 Data Explorer

Allows users to interactively explore, filter, and understand the underlying terrorism dataset.

### ⚙️ Settings

Provides configuration options for the dashboard and application experience.

---

## 🏗️ System Architecture

The application follows a modular architecture consisting of data processing, machine learning, utility functions, and Streamlit-based presentation modules.

```text
                    ┌─────────────────────────┐
                    │     Global Terrorism    │
                    │         Dataset         │
                    └────────────┬────────────┘
                                 │
                                 ▼
                    ┌─────────────────────────┐
                    │     Data Processing &    │
                    │     Feature Preparation  │
                    └────────────┬────────────┘
                                 │
                 ┌───────────────┴────────────────┐
                 │                                │
                 ▼                                ▼
       ┌───────────────────┐           ┌────────────────────┐
       │ Machine Learning  │           │ Exploratory Data   │
       │     Prediction    │           │     Analysis       │
       └─────────┬─────────┘           └──────────┬─────────┘
                 │                                │
                 └───────────────┬────────────────┘
                                 ▼
                    ┌─────────────────────────┐
                    │  Military Intelligence │
                    │       Dashboard         │
                    └────────────┬────────────┘
                                 │
          ┌──────────────────────┼──────────────────────┐
          ▼                      ▼                      ▼
    Threat Mapping        Attack Prediction       Forecasting
          │                      │                      │
          └──────────────────────┼──────────────────────┘
                                 ▼
                       Intelligence Insights
```

---

## 🛠️ Technologies Used

### Programming Language

* **Python**

### Framework

* **Streamlit**

### Data Analysis

* **Pandas**
* **NumPy**

### Machine Learning

* **Scikit-learn**
* Serialized machine learning models using **Pickle/PKL**

### Data Visualization

* Interactive visualization libraries used within the Streamlit dashboard.

### Development Tools

* Visual Studio Code
* Git
* GitHub

---

## 📂 Project Structure

```text
MILITARY-INTELLIGENCE-DASHBOARD/
│
├── .gitignore
├── README.md
├── app.py
├── train_attack_model.py
│
├── data/
│   └── globalterrorism.csv
│
├── models/
│   ├── attack_prediction_model.pkl
│   ├── feature_encoders.pkl
│   └── target_encoder.pkl
│
├── pages/
│   ├── 1_🏠 Home.py
│   ├── 2_🌍 Global_Threat_Map.py
│   ├── 3_🔎Country_Analysis.py
│   ├── 4_🎯 Attack_Prediction.py
│   ├── 5_🚨Threat_Level.py
│   ├── 6_📈Forecasting.py
│   ├── 7_🧠 AI_Intelligence.py
│   ├── 8_📊Data_Explorer.py
│   └── 9_⚙ Setting.py
│
└── utils/
    └── data_loader.py
```

---

## 🧠 Machine Learning Component

The project includes a dedicated machine learning pipeline for attack prediction.

The training process is implemented in:

```text
train_attack_model.py
```

The trained model and supporting encoders are stored as serialized files:

```text
models/
├── attack_prediction_model.pkl
├── feature_encoders.pkl
└── target_encoder.pkl
```

These components are used by the prediction module to process user-provided inputs and generate model-based predictions.

---

## 📊 Dataset

The dashboard uses the **Global Terrorism Dataset** as its primary source of historical terrorism-related incident information.

The dataset is used for:

* Historical trend analysis
* Geographical analysis
* Country-level analysis
* Threat visualization
* Data exploration
* Forecasting
* Machine learning preparation and prediction

> **Note:** The dataset is a large file and is therefore excluded from the GitHub repository because it exceeds GitHub's individual file-size limitation.

---


## 📦 Large Files

Due to GitHub's individual file-size limitation, the following large files are hosted separately:

- `data/globalterrorism.csv` – Global terrorism dataset used for analysis and visualization.
- `models/attack_prediction_model.pkl` – Trained machine learning model used for attack prediction.

### Download Required Files

The complete dataset and trained model can be downloaded from the following Google Drive folder:

👉 **[Download Dataset and Trained Model](https://drive.google.com/drive/folders/14czccqbAiDTIXIIvc5oFwfWFu2-S4pjc?usp=sharing)**

After downloading, place the files in the following locations:

```text
data/
└── globalterrorism.csv

models/
└── attack_prediction_model.pkl

### Required Files

To run the complete application locally, download these files separately and place them in:

```text
data/globalterrorism.csv
models/attack_prediction_model.pkl
```

The smaller supporting model files are included in the repository.


---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/Nithyasri31/MILITARY-INTELLIGENCE-DASHBOARD.git
```

### 2. Navigate to the Project Directory

```bash
cd MILITARY-INTELLIGENCE-DASHBOARD
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

**Windows:**

```bash
venv\Scripts\activate
```

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Application

After installing the required dependencies and placing the large dataset and model files in their respective directories, run:

```bash
streamlit run app.py
```

The application will open in the browser through the local Streamlit server.

---

## 🔄 Application Workflow

```text
User
  │
  ▼
Streamlit Dashboard
  │
  ├── Global Threat Map
  ├── Country Analysis
  ├── Attack Prediction
  ├── Threat Level
  ├── Forecasting
  ├── AI Intelligence
  ├── Data Explorer
  └── Settings
          │
          ▼
   Data Processing
          │
          ▼
 Machine Learning /
 Analytical Modules
          │
          ▼
 Intelligence Insights
```

---

## 🔐 Responsible Use

This project is developed for **academic, educational, and internship purposes**.

The dashboard is intended to demonstrate the application of data analytics, machine learning, visualization, and AI techniques to publicly available historical security data.

Predictions and analytical outputs should be treated as **data-driven insights rather than definitive real-world intelligence or operational decisions**.

---

## 🔮 Future Enhancements

Potential future improvements include:

* Integration of real-time security and incident data sources.
* Advanced anomaly and emerging-threat detection.
* More sophisticated time-series forecasting models.
* Automated model retraining with newly available data.
* Enhanced geospatial intelligence visualization.
* Role-based access and authentication.
* Deployment on a cloud platform.
* Improved AI-assisted analytical capabilities.
* Model performance monitoring and evaluation.

---



## 📜 Disclaimer

This project is intended solely for **academic, educational, and internship demonstration purposes**. It is not designed to replace professional intelligence analysis, security assessment, or operational decision-making systems.
