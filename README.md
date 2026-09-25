# SIH-26231
# 🌾 Krishi Raksha

## AI-Powered Early Detection and Management of Crop Diseases & Pest Infestations

> **Smart India Hackathon 2026 — Problem Statement ID: SIH26131**
> **Theme:** Agriculture, FoodTech & Rural Development
> **Category:** Software
> **Team:** Tech Innovators

---

## 📌 Table of Contents

* [1. Project Overview](#1-project-overview)
* [2. Problem Statement](#2-problem-statement)
* [3. Why This Problem Matters](#3-why-this-problem-matters)
* [4. Our Solution](#4-our-solution)
* [5. Project Objectives](#5-project-objectives)
* [6. Target Users](#6-target-users)
* [7. Key Features](#7-key-features)
* [8. End-to-End Architecture](#8-end-to-end-architecture)
* [9. Complete System Workflow](#9-complete-system-workflow)
* [10. Technology Stack](#10-technology-stack)
* [11. Frontend Architecture](#11-frontend-architecture)
* [12. Backend Architecture](#12-backend-architecture)
* [13. AI/ML Architecture](#13-aiml-architecture)
* [14. Weather and Risk Forecasting](#14-weather-and-risk-forecasting)
* [15. Geospatial Hotspot Detection](#15-geospatial-hotspot-detection)
* [16. Multilingual Advisory](#16-multilingual-advisory)
* [17. Alert Engine](#17-alert-engine)
* [18. Expert Validation](#18-expert-validation)
* [19. Data Flow](#19-data-flow)
* [20. Database Architecture](#20-database-architecture)
* [21. Repository Structure](#21-repository-structure)
* [22. Implementation Plan](#22-implementation-plan)
* [23. Machine Learning Pipeline](#23-machine-learning-pipeline)
* [24. API Architecture](#24-api-architecture)
* [25. Installation](#25-installation)
* [26. Environment Variables](#26-environment-variables)
* [27. Running the Project](#27-running-the-project)
* [28. Example Farmer Journey](#28-example-farmer-journey)
* [29. Agriculture Official Dashboard](#29-agriculture-official-dashboard)
* [30. Security and Privacy](#30-security-and-privacy)
* [31. Testing Strategy](#31-testing-strategy)
* [32. Model Evaluation](#32-model-evaluation)
* [33. Risks and Mitigation](#33-risks-and-mitigation)
* [34. Current Project Status](#34-current-project-status)
* [35. Future Scope](#35-future-scope)
* [36. Limitations](#36-limitations)
* [37. Research and Datasets](#37-research-and-datasets)
* [38. Hackathon Demo Flow](#38-hackathon-demo-flow)
* [39. Team Responsibilities](#39-team-responsibilities)
* [40. Frequently Asked Questions](#40-frequently-asked-questions)
* [41. Final Architecture Summary](#41-final-architecture-summary)
* [42. Disclaimer](#42-disclaimer)

---

# 1. 🌱 Project Overview

**Krishi Raksha** is an AI-powered crop-health decision-support platform designed for the **early detection and management of crop diseases and pest infestations**.

The system combines:

* 📷 Crop image analysis
* 🐛 Pest detection
* 🌦️ Weather information
* 🌱 Crop and soil context
* 🤖 Artificial Intelligence / Machine Learning
* 📈 Risk forecasting
* 🗺️ Geospatial hotspot monitoring
* 🔔 Farm-level alerts
* 🗣️ Multilingual advisory
* 👨‍🌾 Farmer application
* 🏛️ Agriculture official dashboard
* 👨‍🔬 Expert validation

The main goal is to move crop-health management from:

> **Reactive detection → Proactive decision support**

Instead of waiting until a disease or pest infestation has spread significantly, Krishi Raksha aims to help identify potential problems earlier and provide understandable information to farmers and agriculture officials.

---

# 2. 🚨 Problem Statement

Farmers may identify crop diseases and pest infestations only after visible symptoms or damage become significant.

This creates several challenges:

* Disease may already have spread.
* Pest infestation may increase rapidly.
* Farmers may not have immediate access to experts.
* Manual diagnosis can take time.
* Weather and crop-stage information may not be considered together.
* Incorrect identification can lead to inappropriate action.
* Agriculture officials may not have a real-time regional overview.

### Core Problem

The key question we are trying to solve is:

> **How can we detect crop diseases and pest infestations earlier and convert the detection into useful, farm-level decision support?**

---

# 3. 🌾 Why This Problem Matters

A crop-health problem is not only an image-classification problem.

A useful agricultural system needs to answer:

### Question 1 — What is happening?

Use computer vision to analyse the crop image.

### Question 2 — What is the risk?

Combine the visual result with environmental and historical context.

### Question 3 — What should happen next?

Provide understandable advisory and alerts.

### Question 4 — Is this problem appearing in other locations?

Use geospatial information to identify possible hotspots.

Therefore, Krishi Raksha is designed as an **end-to-end crop-health decision-support system**.

---

# 4. 💡 Our Solution

Krishi Raksha follows this basic pipeline:

```text
Capture
   ↓
Process
   ↓
Detect
   ↓
Analyse
   ↓
Forecast Risk
   ↓
Generate Advisory
   ↓
Alert
   ↓
Map Hotspots
   ↓
Expert Validation
```

### Farmer Side

A farmer can:

1. Open the Krishi Raksha application.
2. Capture or upload an image.
3. Select the crop.
4. Provide relevant information.
5. Submit the scan.
6. Receive an AI-based result.
7. View risk information.
8. Receive multilingual advisory.
9. Receive alerts when appropriate.

### Official Side

Agriculture officials can:

1. View reported cases.
2. Monitor risk levels.
3. View geographic distribution.
4. Identify possible hotspots.
5. Review trends.
6. Send cases for expert validation.

---

# 5. 🎯 Project Objectives

The major objectives are:

1. Early detection of crop diseases.
2. Detection of pest infestations.
3. Automated first-level image analysis.
4. Integration of weather information.
5. Integration of crop and soil context.
6. Risk forecasting using historical information.
7. Multilingual farmer communication.
8. Farm-level alerts.
9. Geographic hotspot identification.
10. Agriculture-official monitoring.
11. Expert validation of uncertain cases.
12. Creation of a scalable architecture for future deployment.

---

# 6. 👥 Target Users

## 👨‍🌾 Farmers

Farmers are the primary users.

They can:

* Scan crops.
* Upload images.
* View predictions.
* Check risk.
* Receive alerts.
* Read/listen to advisory.
* View previous scans.

---

## 🧑‍🌾 Extension Workers

Extension workers can:

* Monitor farmer reports.
* Identify areas requiring attention.
* Prioritize field visits.
* Validate cases.

---

## 🏛️ Agriculture Officials

Officials can:

* Monitor regional disease/pest activity.
* View possible hotspots.
* Analyse trends.
* Review alerts.
* Monitor expert validation.

---

## 👨‍🔬 Agricultural Experts

Experts can:

* Review uncertain predictions.
* Confirm or reject predictions.
* Correct incorrect classifications.
* Provide feedback.

---

# 7. 🚀 Key Features

## 7.1 AI Crop Disease Detection

The farmer uploads/captures a crop image.

The AI model analyses the image and predicts the supported disease class.

---

## 7.2 Pest Detection

YOLO-based object detection can identify and localize pests in images.

---

## 7.3 Weather Risk Analysis

Weather information is combined with crop-health information to provide contextual risk analysis.

---

## 7.4 Risk Forecasting

A time-series forecasting component using LSTM is proposed for analysing historical environmental information and supporting future risk estimation.

---

## 7.5 Multilingual Advisory

The system presents information in farmer-friendly language and supports regional-language communication.

---

## 7.6 Smart Alerts

The alert engine generates alerts when configured conditions indicate that a case requires attention.

---

## 7.7 Geospatial Hotspot Monitoring

Reports containing geographic information can be aggregated to identify possible disease or pest clusters.

---

## 7.8 Agriculture Dashboard

Officials can monitor:

* Reports
* Alerts
* Risk
* Hotspots
* Trends
* Expert validation

---

## 7.9 Expert Validation

AI predictions can be reviewed by authorized experts when confidence is low or the case requires additional verification.

---

# 8. 🏗️ End-to-End Architecture

## High-Level Architecture

```text
                         KRISHI RAKSHA
                              │
                              ▼
                 ┌────────────────────────┐
                 │      DATA SOURCES      │
                 └────────────────────────┘
                    │                 │
          ┌─────────┴────────┐   ┌────┴─────────┐
          │ Smartphone Camera│   │ IoT / Pest   │
          │ / Image Upload   │   │ Trap Sensors │
          └─────────┬────────┘   └────┬─────────┘
                    │                 │
                    └────────┬────────┘
                             ▼
                  ┌──────────────────────┐
                  │    REACT FRONTEND    │
                  │                      │
                  │ Farmer App + Admin   │
                  │ Dashboard            │
                  └──────────┬───────────┘
                             │
                             ▼
                   ┌───────────────────┐
                   │     FASTAPI       │
                   │   BACKEND / API   │
                   └─────────┬─────────┘
                             │
             ┌───────────────┼────────────────┐
             │               │                │
             ▼               ▼                ▼
      ┌────────────┐  ┌─────────────┐  ┌─────────────┐
      │ AI / ML    │  │ Weather API │  │ Crop / Soil │
      │ Pipeline   │  │             │  │ Context     │
      └─────┬──────┘  └──────┬──────┘  └──────┬──────┘
            │                │                │
            └────────────────┼────────────────┘
                             ▼
                  ┌──────────────────────┐
                  │    RISK ENGINE       │
                  │ + FORECASTING        │
                  └──────────┬───────────┘
                             │
               ┌─────────────┼─────────────┐
               ▼             ▼             ▼
        ┌────────────┐ ┌───────────┐ ┌────────────┐
        │ Advisory   │ │ Alert     │ │ Geospatial │
        │ Engine     │ │ Engine    │ │ Engine     │
        └─────┬──────┘ └─────┬─────┘ └──────┬─────┘
              │              │              │
              └──────────────┼──────────────┘
                             ▼
                  ┌──────────────────────┐
                  │ PostgreSQL + PostGIS │
                  │ + Object Storage     │
                  └──────────┬───────────┘
                             │
                             ▼
                  ┌──────────────────────┐
                  │ OFFICIAL DASHBOARD   │
                  │ + HOTSPOT MAP        │
                  └──────────────────────┘
```

---

# 9. 🔄 Complete System Workflow

## Step 1 — Capture

The farmer provides:

```text
Crop Image
Crop Type
Crop Stage
Location
Optional Sensor Information
```

---

## Step 2 — React Frontend

The React application:

```text
Open Camera / Upload
        ↓
Select Crop
        ↓
Enter Required Information
        ↓
Validate Input
        ↓
Send Request
```

---

## Step 3 — FastAPI Backend

FastAPI receives:

```text
Image
+
Crop Information
+
Location
+
Crop Stage
+
Sensor Data
```

The backend validates the request.

---

## Step 4 — Image Preprocessing

Possible preprocessing:

```text
Image
 ↓
Format Validation
 ↓
Resize
 ↓
Normalization
 ↓
Quality Check
 ↓
ML Input
```

---

## Step 5 — AI Detection

The image is passed to the appropriate model.

### Classification

```text
Image
 ↓
CNN / EfficientNet
 ↓
Disease Class
 ↓
Confidence
```

### Object Detection

```text
Image
 ↓
YOLOv8
 ↓
Object / Pest
 ↓
Bounding Box
 ↓
Confidence
```

---

## Step 6 — Context Collection

The system collects relevant information:

```text
Weather
Crop Stage
Soil Information
Location
Historical Reports
```

---

## Step 7 — Risk Analysis

The system combines:

```text
AI Prediction
+
Weather
+
Crop Stage
+
Environmental Context
+
Historical Data
```

to produce contextual risk information.

---

## Step 8 — Risk Forecasting

Historical/time-series data can be processed using LSTM.

```text
Historical Data
      ↓
Sequence Formation
      ↓
LSTM
      ↓
Risk Forecast
```

---

## Step 9 — Advisory

The advisory engine converts technical information into a farmer-friendly result.

Example:

```text
Possible Threat:
Tomato Early Blight

Confidence:
Model Confidence

Risk:
High / Medium / Low

Next Step:
Follow validated agricultural guidance
and inspect nearby plants.

Language:
English / Regional Language
```

---

## Step 10 — Alert

The alert engine evaluates the configured conditions.

```text
Prediction
    +
Confidence
    +
Risk
    ↓
Alert Rules
    ↓
Alert / Normal Result / Expert Review
```

---

## Step 11 — Store Report

The result is stored with:

```text
Crop
Threat
Confidence
Risk
Location
Timestamp
Image Reference
Model Version
```

---

## Step 12 — Hotspot Analysis

Multiple geographically related reports can be analysed.

```text
Farmer A ─┐
Farmer B ─┼──► Geographic Analysis ──► Possible Hotspot
Farmer C ─┘
```

---

## Step 13 — Expert Validation

Uncertain or important cases can be sent to an expert.

```text
AI Prediction
      ↓
Confidence Check
      ↓
Expert Review
      ↓
Validated Result
```

---

## Step 14 — Official Dashboard

Officials see:

```text
Reports
Alerts
Risk Levels
Maps
Hotspots
Trends
Validation Status
```

---

# 10. 🧰 Technology Stack

| Layer               | Technology               |
| ------------------- | ------------------------ |
| Frontend            | **React**                |
| Dashboard           | React                    |
| Backend             | FastAPI                  |
| Additional Backend  | Node.js where required   |
| Programming         | Python + JavaScript      |
| ML                  | TensorFlow, scikit-learn |
| Image Models        | CNN, EfficientNet        |
| Object Detection    | YOLOv8                   |
| Edge ML             | TensorFlow Lite          |
| Forecasting         | LSTM                     |
| Database            | PostgreSQL               |
| Geospatial Database | PostGIS                  |
| Storage             | Firebase / S3            |
| Maps                | Leaflet                  |
| Visualization       | Grafana                  |
| Weather             | IMD Weather API          |
| Multilingual        | Bhashini API             |
| Version Control     | Git + GitHub             |

### Frontend Change

> **The current architecture uses React instead of Flutter.**

The previous presentation contained Flutter as the frontend technology; React is now the selected frontend technology for the project.

---

# 11. ⚛️ Frontend Architecture

The React application has two major interfaces.

```text
React
│
├── Farmer Application
│
└── Agriculture Official Dashboard
```

---

## Farmer Application

Suggested pages:

```text
/login
/register
/dashboard
/scan
/result
/weather
/advisory
/alerts
/history
/profile
```

---

## Official Dashboard

Suggested pages:

```text
/admin/login
/admin/dashboard
/admin/map
/admin/reports
/admin/alerts
/admin/validation
/admin/analytics
```

---

## React Component Structure

```text
src/
│
├── components/
│   ├── Navbar/
│   ├── Sidebar/
│   ├── CameraUpload/
│   ├── ScanResult/
│   ├── WeatherCard/
│   ├── RiskCard/
│   ├── AdvisoryCard/
│   ├── AlertCard/
│   └── Map/
│
├── pages/
│   ├── Login/
│   ├── Dashboard/
│   ├── Scan/
│   ├── Result/
│   ├── History/
│   └── Admin/
│
├── services/
│   ├── api.js
│   ├── auth.js
│   ├── prediction.js
│   └── weather.js
│
├── hooks/
├── context/
├── utils/
├── assets/
├── App.jsx
└── main.jsx
```

---

# 12. ⚙️ Backend Architecture

FastAPI acts as the primary backend/API layer.

```text
React
  │
  │ REST API
  ▼
FastAPI
  │
  ├── Authentication
  ├── Image Upload
  ├── Prediction Service
  ├── Weather Service
  ├── Risk Service
  ├── Advisory Service
  ├── Alert Service
  ├── Geospatial Service
  └── Dashboard Service
       │
       ├── PostgreSQL
       ├── PostGIS
       ├── Object Storage
       └── ML Models
```

---

# 13. 🤖 AI/ML Architecture

## 13.1 CNN

CNN stands for **Convolutional Neural Network**.

It learns visual patterns such as:

* Edges
* Textures
* Shapes
* Patterns
* Disease-related visual features

---

## 13.2 EfficientNet

EfficientNet is used as an efficient deep-learning architecture for image classification/feature extraction.

The objective is to balance:

```text
Accuracy
+
Model Size
+
Computational Cost
```

---

## 13.3 YOLOv8

YOLO is an object-detection architecture.

It can provide:

```text
Object Class
+
Location
+
Confidence
```

This is useful for pest detection where the location of an object within the image matters.

---

## 13.4 TensorFlow

TensorFlow can be used for:

* Model development
* Training
* Evaluation
* Model export
* Inference integration

---

## 13.5 TensorFlow Lite

TensorFlow Lite can be used to deploy optimized models for lightweight or edge inference.

This is particularly useful for environments where network connectivity is limited.

---

## 13.6 scikit-learn

scikit-learn can support:

* Data preprocessing
* Classical ML experiments
* Evaluation
* Feature processing
* Supporting analytics

---

# 14. 🌦️ Weather and Risk Forecasting

Disease and pest risk is not determined only by the image.

Environmental conditions can provide additional context.

Potential inputs:

```text
Temperature
Humidity
Rainfall
Weather Trend
Location
Crop Stage
Historical Reports
```

---

## Risk Pipeline

```text
Weather API
      ↓
Data Cleaning
      ↓
Feature Engineering
      ↓
Historical Sequence
      ↓
LSTM
      ↓
Risk Forecast
```

The risk forecast should be treated as a model output requiring validation before being used for high-impact agricultural decisions.

---

# 15. 🗺️ Geospatial Hotspot Detection

Location is an important part of the system.

Each report can contain:

```text
Latitude
Longitude
Threat Type
Crop
Risk
Confidence
Timestamp
```

PostGIS is used to support geospatial storage and queries.

---

## Hotspot Flow

```text
Reports
   ↓
Coordinates
   ↓
PostGIS
   ↓
Spatial Queries / Aggregation
   ↓
Potential Hotspot
   ↓
Leaflet Map
   ↓
Official Dashboard
```

A hotspot represents a **possible geographic cluster** and should not automatically be treated as proof that an entire region is infected.

---

# 16. 🗣️ Multilingual Advisory

A farmer should not have to understand complex ML terminology.

Therefore:

```text
AI Result
   ↓
Advisory Rules
   ↓
Simple Explanation
   ↓
Language Conversion
   ↓
Text / Voice
   ↓
Farmer
```

Potential supported languages can be expanded according to deployment requirements.

Bhashini is included in the technical direction for multilingual communication.

---

# 17. 🔔 Alert Engine

The alert engine prevents every prediction from becoming an immediate high-priority alert.

Conceptual flow:

```text
AI Prediction
      ↓
Confidence
      ↓
Risk Level
      ↓
Alert Rules
      ↓
┌──────────────┬───────────────┐
│              │               │
▼              ▼               ▼
Alert       Normal Result   Expert Review
```

Example conceptual rule:

```text
IF confidence >= threshold
AND risk >= threshold
THEN generate alert
```

Thresholds should be selected through testing and validation.

---

# 18. 👨‍🔬 Expert Validation

AI predictions should not automatically be considered perfect.

The system therefore supports an expert-validation workflow.

```text
AI Prediction
      ↓
Confidence Check
      ↓
Low Confidence / Important Case
      ↓
Expert Dashboard
      ↓
Review Image + Prediction
      ↓
Confirm / Reject / Correct
      ↓
Validated Record
```

Expert feedback can also become useful future training data, subject to appropriate data-management practices.

---

# 19. 🔄 Data Flow

```text
                 FARMER
                    │
                    ▼
             ┌─────────────┐
             │ React App   │
             └──────┬──────┘
                    │
          Image + Metadata
                    │
                    ▼
             ┌─────────────┐
             │  FastAPI    │
             └──────┬──────┘
                    │
       ┌────────────┼────────────┐
       │            │            │
       ▼            ▼            ▼
     AI/ML       Weather      Database
       │            │            │
       └────────────┼────────────┘
                    ▼
             ┌─────────────┐
             │ Risk Engine │
             └──────┬──────┘
                    │
       ┌────────────┼────────────┐
       ▼            ▼            ▼
   Advisory       Alert       Geospatial
       │            │            │
       └────────────┼────────────┘
                    ▼
             ┌─────────────┐
             │ React UI    │
             └──────┬──────┘
                    │
          ┌─────────┴─────────┐
          ▼                   ▼
       Farmer              Officials
```

---

# 20. 🗄️ Database Architecture

## Users

```text
users
-----
id
name
phone/email
role
language
created_at
```

---

## Farms

```text
farms
-----
id
user_id
farm_name
crop
crop_stage
location
created_at
```

---

## Crop Scans

```text
crop_scans
----------
id
farm_id
image_url
crop
timestamp
latitude
longitude
status
```

---

## Predictions

```text
predictions
-----------
id
scan_id
threat_type
predicted_class
confidence
risk_level
model_version
created_at
```

---

## Weather Records

```text
weather_records
---------------
id
location
temperature
humidity
rainfall
timestamp
source
```

---

## Alerts

```text
alerts
------
id
user_id
prediction_id
risk_level
message
status
created_at
```

---

## Expert Validation

```text
expert_validations
------------------
id
prediction_id
expert_id
decision
corrected_class
comments
validated_at
```

---

# 21. 📁 Repository Structure

Recommended GitHub structure:

```text
krishi-raksha/
│
├── README.md
├── LICENSE
├── .gitignore
├── .env.example
├── docker-compose.yml
│
├── frontend/
│   ├── package.json
│   ├── public/
│   └── src/
│       ├── components/
│       ├── pages/
│       ├── layouts/
│       ├── services/
│       ├── hooks/
│       ├── context/
│       ├── utils/
│       ├── assets/
│       ├── App.jsx
│       └── main.jsx
│
├── backend/
│   ├── requirements.txt
│   ├── app/
│   │   ├── main.py
│   │   ├── config.py
│   │   ├── database.py
│   │   ├── models/
│   │   ├── schemas/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── middleware/
│   │   └── utils/
│   └── tests/
│
├── ml/
│   ├── datasets/
│   ├── notebooks/
│   ├── preprocessing/
│   ├── training/
│   ├── evaluation/
│   ├── inference/
│   ├── models/
│   └── requirements.txt
│
├── data/
│   ├── sample/
│   └── README.md
│
├── docs/
│   ├── architecture/
│   ├── api/
│   ├── database/
│   ├── ml/
│   ├── deployment/
│   └── screenshots/
│
├── scripts/
│   ├── setup.sh
│   ├── seed_db.py
│   └── download_models.py
│
└── deployment/
    ├── Dockerfile
    ├── nginx/
    └── cloud/
```

---

# 22. 🛠️ Implementation Plan

## Phase 1 — Research

* Understand problem statement.
* Identify target crops.
* Identify target diseases/pests.
* Study available datasets.
* Study agricultural guidance.
* Identify weather variables.

---

## Phase 2 — Dataset Preparation

```text
Dataset Collection
       ↓
Data Cleaning
       ↓
Label Verification
       ↓
Preprocessing
       ↓
Train / Validation / Test
```

---

## Phase 3 — AI Model

Develop:

* Disease classifier
* Pest detector
* Risk forecasting component

---

## Phase 4 — Backend

Develop:

* Authentication
* Image upload
* Prediction API
* Weather API
* Risk API
* Advisory API
* Alert API
* Geospatial API

---

## Phase 5 — React Frontend

Develop:

* Login
* Dashboard
* Crop scan
* Prediction result
* Weather
* Risk
* Advisory
* Alerts
* History

---

## Phase 6 — Official Dashboard

Develop:

* Analytics
* Map
* Hotspots
* Reports
* Alerts
* Expert validation

---

## Phase 7 — Integration

Connect:

```text
React
+
FastAPI
+
ML
+
Weather
+
Database
+
Geospatial
```

---

## Phase 8 — Testing

Perform:

* Unit testing
* API testing
* ML testing
* Integration testing
* UI testing
* Field testing

---

## Phase 9 — Pilot

Test with representative:

* Crops
* Diseases
* Pest conditions
* Devices
* Lighting conditions
* Network conditions
* Geographic areas

---

# 23. 🤖 Machine Learning Pipeline

```text
Raw Dataset
     ↓
Data Cleaning
     ↓
Label Verification
     ↓
Train / Validation / Test Split
     ↓
Image Preprocessing
     ↓
Data Augmentation
     ↓
Model Training
     ↓
Validation
     ↓
Hyperparameter Tuning
     ↓
Final Evaluation
     ↓
Model Export
     ↓
Inference Service
     ↓
Production / Prototype
```

---

# 24. 🔌 API Architecture

## Authentication

```http
POST /api/auth/register
POST /api/auth/login
POST /api/auth/logout
```

## Crop Scan

```http
POST /api/scans
GET /api/scans/{scan_id}
GET /api/scans/history
```

## Prediction

```http
POST /api/predict
GET /api/predictions/{prediction_id}
```

## Weather

```http
GET /api/weather
GET /api/weather/risk
```

## Advisory

```http
GET /api/advisory/{prediction_id}
```

## Alerts

```http
GET /api/alerts
POST /api/alerts/{alert_id}/read
```

## Geospatial

```http
GET /api/hotspots
GET /api/reports/nearby
```

## Expert Validation

```http
GET /api/validation/pending
POST /api/validation/{prediction_id}
```

## Dashboard

```http
GET /api/dashboard/summary
GET /api/dashboard/trends
GET /api/dashboard/map
```

---

# 25. 💻 Installation

## Prerequisites

Install:

* Git
* Node.js
* npm
* Python 3.x
* PostgreSQL
* PostGIS
* Optional Docker

---

## Clone Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>

cd krishi-raksha
```

---

## Frontend

```bash
cd frontend

npm install

npm run dev
```

---

## Backend

Create virtual environment:

### Windows

```bash
python -m venv venv

venv\Scripts\activate
```

### Linux/macOS

```bash
python3 -m venv venv

source venv/bin/activate
```

Install packages:

```bash
cd backend

pip install -r requirements.txt
```

Run FastAPI:

```bash
uvicorn app.main:app --reload
```

---

# 26. 🔐 Environment Variables

Create:

```text
.env
```

Example:

```env
DATABASE_URL=postgresql://username:password@localhost:5432/krishi_raksha

WEATHER_API_KEY=your_weather_api_key

BHASHINI_API_KEY=your_bhashini_api_key

MODEL_PATH=./ml/models/model

STORAGE_BUCKET=your_bucket

JWT_SECRET=your_secret

ENVIRONMENT=development
```

### Important

Never commit:

```text
.env
API Keys
Passwords
JWT Secrets
Private Credentials
```

to GitHub.

Use:

```text
.env.example
```

instead.

---

# 27. ▶️ Running the Project

## Start Backend

```bash
cd backend

uvicorn app.main:app --reload
```

---

## Start Frontend

```bash
cd frontend

npm run dev
```

---

## Database

Create PostgreSQL database:

```text
krishi_raksha
```

Enable PostGIS:

```sql
CREATE EXTENSION postgis;
```

---

# 28. 👨‍🌾 Example Farmer Journey

### Scenario

A farmer notices unusual spots on a tomato plant.

### Step 1

The farmer opens Krishi Raksha.

### Step 2

Selects:

> **Scan Crop**

### Step 3

Captures/uploads a leaf image.

### Step 4

Selects:

> Tomato

### Step 5

React sends the information to FastAPI.

### Step 6

The AI pipeline analyses the image.

### Step 7

The system returns:

```text
Possible Threat
Confidence
```

### Step 8

Weather/context information is retrieved.

### Step 9

The risk engine analyses contextual risk.

### Step 10

The advisory engine generates a simple explanation.

### Step 11

The farmer receives the information in a supported language.

### Step 12

If configured conditions are met, an alert is generated.

### Step 13

The report is stored with location information.

### Step 14

Related reports can contribute to a potential hotspot.

### Step 15

An official/expert can review the case.

---

# 29. 🏛️ Agriculture Official Dashboard

## Dashboard Overview

Display:

```text
Total Reports
Active Alerts
High-Risk Cases
Pending Validation
Potential Hotspots
```

---

## Map

Display:

* Disease reports
* Pest reports
* Risk levels
* Potential hotspots
* Location
* Time filters
* Crop filters

---

## Analytics

Possible analytics:

```text
Cases Over Time
Disease Distribution
Pest Distribution
Crop-Wise Cases
Region-Wise Cases
Risk Distribution
```

---

## Expert Validation

Experts can:

```text
View Image
View Prediction
View Confidence
Confirm
Reject
Correct
Add Comments
```

---

# 30. 🔒 Security and Privacy

The application should use role-based access.

## Farmer

```text
Own Data
Own Scans
Own Alerts
```

## Expert

```text
Assigned Validation Cases
```

## Official

```text
Regional Monitoring
```

## Admin

```text
System Management
```

Security practices:

* HTTPS
* Secure authentication
* Password hashing
* Authorization
* Input validation
* File validation
* Rate limiting
* Database access control
* Secure API keys

---

# 31. 🧪 Testing Strategy

## Unit Testing

Test individual functions.

---

## API Testing

Test:

* Valid requests
* Invalid requests
* Authentication
* Image uploads
* API failures

---

## ML Testing

Test:

* Correct images
* Incorrect images
* Low-quality images
* Different lighting
* Different backgrounds
* Different crop stages

---

## Integration Testing

Test the entire chain:

```text
React
 ↓
FastAPI
 ↓
ML
 ↓
Database
 ↓
Response
```

---

## Field Testing

Evaluate under:

* Different phones
* Different lighting
* Different locations
* Different crops
* Different disease stages
* Different network conditions

---

# 32. 📊 Model Evaluation

Accuracy should not be the only metric.

Use:

### Accuracy

Overall percentage of correct predictions.

### Precision

How many predicted positives are actually positive?

### Recall

How many actual positive cases were detected?

### F1-score

Balance between precision and recall.

### Confusion Matrix

Shows class-wise errors.

### mAP

Important for object-detection models.

### Inference Time

Measures how quickly the model generates a result.

### Field Performance

Compare model performance between controlled datasets and real-world images.

---

# 33. ⚠️ Risks and Mitigation

| Risk             | Problem                      | Mitigation                               |
| ---------------- | ---------------------------- | ---------------------------------------- |
| Poor image       | Incorrect prediction         | Image-quality check                      |
| Low light        | Poor features                | Capture guidance / preprocessing         |
| Poor network     | Cloud unavailable            | Offline-capable inference where feasible |
| False positive   | Wrong intervention           | Confidence threshold + validation        |
| False negative   | Threat missed                | Recall-focused evaluation                |
| Language barrier | Poor understanding           | Regional language                        |
| Dataset bias     | Poor field performance       | Diverse field data                       |
| Unknown disease  | Wrong known-class prediction | Uncertain state                          |
| Sensor failure   | Missing data                 | Fallback inputs                          |
| API failure      | Missing weather              | Retry/cache strategy                     |

---

# 34. 📌 Current Project Status

The project is being developed as a **Smart India Hackathon 2026 prototype**.

Current architecture includes:

* React frontend
* FastAPI backend
* AI/ML pipeline
* Weather integration
* Risk analysis
* Geospatial monitoring
* Multilingual advisory
* Alert engine
* Agriculture dashboard
* Expert validation workflow

### Important

Not every architectural component should be described as production-ready unless it has actually been implemented and tested.

As development progresses, this section should be updated with:

```text
✅ Implemented
🟡 In Progress
🔵 Planned
❌ Not Started
```

---

# 35. 🔮 Future Scope

## More Crops

Expand the number of supported crops.

## More Diseases

Add more disease classes.

## More Pest Classes

Expand pest detection.

## Edge AI

Deploy optimized models directly on supported devices.

## More IoT Sensors

Potential integrations:

```text
Soil Moisture
Temperature
Humidity
Pest Traps
```

## Better Forecasting

Use more historical environmental and crop-health data.

## Expert Feedback Loop

Use validated cases for future model improvement.

## Large-Scale Deployment

Scale to larger numbers of farmers and geographic regions.

---

# 36. ❗ Limitations

## Dataset Limitation

Public datasets may not perfectly represent real field conditions.

## Image Quality

Blur, lighting, background and occlusion can affect predictions.

## Model Coverage

The model can only reliably identify classes represented in the validated training data.

## Weather Uncertainty

Weather and risk forecasts are not guaranteed predictions.

## Network Dependency

Some cloud-based functionality requires connectivity.

## AI Errors

AI can produce incorrect predictions.

## Expert Validation

High-impact cases should be verified appropriately.

---

# 37. 📚 Research and Datasets

The project research direction includes:

### PlantVillage

Crop-disease image dataset.

### IP102

Pest-image dataset.

### IMD Weather API

Weather information.

### Bhashini

Multilingual communication support.

### FAO IPM Guidelines

Agricultural integrated-pest-management guidance reference.

### YOLOv8

Object detection technology.

### TensorFlow

Machine-learning framework.

---

# 38. 🎬 Hackathon Demo Flow

For the final demonstration, use this sequence.

## Demo 1 — Farmer Application

Open:

```text
Farmer Dashboard
```

---

## Demo 2 — Crop Scan

Upload/capture a sample image.

---

## Demo 3 — AI Detection

Show:

```text
Disease/Pest
Confidence
```

---

## Demo 4 — Weather

Show:

```text
Current Conditions
Risk Information
```

---

## Demo 5 — Advisory

Show:

```text
Threat
Risk
Advisory
Language
```

---

## Demo 6 — Alert

Show an alert generated according to configured rules.

---

## Demo 7 — Official Dashboard

Show:

```text
Reports
Analytics
Map
Hotspots
```

---

## Demo 8 — Expert Validation

Show:

```text
AI Prediction
      ↓
Expert Review
      ↓
Validated Result
```

---

# 39. 👨‍💻 Team Responsibilities

## Frontend Developer

Responsible for:

* React
* UI/UX
* Farmer interface
* Dashboard
* API integration

---

## Backend Developer

Responsible for:

* FastAPI
* REST APIs
* Authentication
* Database
* Business logic

---

## AI/ML Developer

Responsible for:

* Dataset
* Preprocessing
* Training
* YOLO
* EfficientNet
* Evaluation
* Inference

---

## Integration / Research Developer

Responsible for:

* Weather
* Risk engine
* Geospatial system
* Multilingual support
* Testing
* Documentation

---

# 40. ❓ Frequently Asked Questions

## Is Krishi Raksha only an image classifier?

No.

It combines image analysis with weather/context, risk forecasting, advisory, alerts and geospatial monitoring.

---

## Why AI?

AI can automate first-level image analysis and provide faster identification of supported crop-health conditions.

---

## Does AI replace agricultural experts?

No.

The system is a decision-support tool.

Expert validation remains important for uncertain or high-impact cases.

---

## Can the system identify every disease?

No.

Reliable detection depends on the crops, diseases and pest classes represented in the training and validation data.

---

## Why use YOLO?

YOLO is suitable for object detection and localization, which is useful for pest detection.

---

## Why use EfficientNet?

EfficientNet provides an efficient deep-learning architecture suitable for image classification/feature extraction.

---

## Why use LSTM?

LSTM is designed for sequential/time-series information and can support temporal risk forecasting.

---

## Why use PostGIS?

PostGIS adds geospatial functionality to PostgreSQL.

This allows location-based reports and spatial analysis.

---

## Why use React?

React is the current frontend technology for Krishi Raksha.

It replaces Flutter from the earlier architecture.

---

## What if the farmer has no internet?

The architecture supports the possibility of lightweight local inference using TensorFlow Lite, with synchronization when connectivity becomes available.

Cloud-dependent services will still require connectivity.

---

## What if AI gives the wrong result?

The system should use confidence thresholds, uncertain states and expert validation instead of treating every AI prediction as absolute truth.

---

## What is the biggest technical challenge?

A major challenge is **real-world generalization**.

A model trained on public datasets may perform differently on:

* Different phones
* Different lighting
* Different crop varieties
* Different backgrounds
* Different geographic regions
* Different disease stages

Therefore, field validation is essential.

---

# 41. 🏆 Final Architecture Summary

The complete Krishi Raksha architecture can be summarized as:

```text
                ┌───────────────────┐
                │      FARMER       │
                └─────────┬─────────┘
                          │
                          ▼
                ┌───────────────────┐
                │   REACT FRONTEND  │
                └─────────┬─────────┘
                          │
                          ▼
                ┌───────────────────┐
                │      FASTAPI      │
                │      BACKEND      │
                └─────────┬─────────┘
                          │
          ┌───────────────┼────────────────┐
          │               │                │
          ▼               ▼                ▼
      ┌────────┐    ┌────────────┐   ┌────────────┐
      │ AI/ML  │    │  Weather   │   │ Crop/Soil  │
      │Models  │    │    API     │   │  Context   │
      └────┬───┘    └─────┬──────┘   └─────┬──────┘
           │              │                │
           └──────────────┼────────────────┘
                          ▼
                 ┌─────────────────┐
                 │  RISK ENGINE    │
                 │ + LSTM FORECAST │
                 └────────┬────────┘
                          │
             ┌────────────┼────────────┐
             ▼            ▼            ▼
        ┌──────────┐ ┌─────────┐ ┌────────────┐
        │ Advisory │ │ Alerts  │ │ Geospatial │
        └────┬─────┘ └────┬────┘ └──────┬─────┘
             │            │             │
             └────────────┼─────────────┘
                          ▼
                ┌────────────────────┐
                │ PostgreSQL/PostGIS │
                └─────────┬──────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ OFFICIAL DASHBOARD │
                │ + HOTSPOT MAP      │
                └────────────────────┘
```

### One-Line Architecture

> **React → FastAPI → AI/ML + Weather + Context → Risk Engine → Advisory + Alerts → PostgreSQL/PostGIS → Official Dashboard**

### Complete Data Journey

> **Capture → Process → Detect → Analyse → Forecast → Advise → Alert → Map → Validate**

---

# 42. ⚖️ Disclaimer

Krishi Raksha is a prototype/decision-support project.

AI predictions may contain errors and should not automatically be treated as definitive agricultural diagnoses.

Crop disease and pest management decisions should be validated against appropriate agricultural expertise and applicable local guidance.

Any pesticide, chemical or treatment-related recommendation must follow applicable product labels, agricultural regulations and qualified expert advice.

---

# 🌾 Final Project Statement

> **Krishi Raksha is an AI-powered crop-health decision-support system that combines computer vision, environmental context, risk forecasting, multilingual advisory and geospatial monitoring to support early detection and management of crop diseases and pest infestations.**

---


