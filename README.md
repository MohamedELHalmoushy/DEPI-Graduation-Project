🇪🇬 GeoLens: AI-Powered Land Type Classification for Egypt Vision 2030
🚀 Project Overview
GeoLens is an AI and Remote Sensing solution designed to combat rapid agricultural land loss in Egypt, directly supporting Egypt Vision 2030 for sustainable development.

This project utilizes advanced Deep Learning models (CNN, U-Net) to automatically classify land types (Agriculture, Urban, Water, Desert) from Sentinel-2 satellite imagery. The core output is an interactive dashboard providing policymakers, environmental analysts, and urban planners with real-time data on land-use changes and a 5-year agricultural land forecast.

🎯 Core Objectives
High-Accuracy Classification: Deploy a U-Net/CNN model to classify Sentinel-2 images into 10 land categories (Forest, Residential, Annual Crop, etc.).

Change Detection: Monitor and quantify land-use transformations between 2015 and 2023.

Future Forecasting: Implement Time-Series models (Prophet/ARIMA) to predict agricultural land expansion or shrinkage for the next five years.

Interactive Dashboard: Deliver a user-friendly web platform using Leaflet.js for map visualization and SerpAPI for real-time contextual information retrieval.

🛠️ Technology Stack
This project adopts an MVC (Model-View-Controller) architecture to ensure modularity, scalability, and maintainability.

Layer

Technology

Purpose

Model (AI)

Python, TensorFlow/Keras

Training and serving the CNN and U-Net classification models.

Controller (Backend)

Flask (Python)

Handles API routing, prediction requests, and integration with the Search API.

View (Frontend)

HTML, CSS, JavaScript, Leaflet.js

Interactive dashboard, geospatial visualization, and UI/UX.

Data Source

Sentinel-2 Images (EuroSAT)

The primary satellite imagery dataset for model training.

Search Integration

SerpAPI

Retrieves relevant, real-time environmental insights based on image location/classification.

Deployment

Google Colab (GPU)

Primary environment for model training and initial deployment.

⚙️ Installation and Setup
Follow these steps to set up the project locally.

1. Prerequisites
You will need the following installed:

Python 3.8+

Git

TensorFlow / Keras (for the AI model component)

A SerpAPI Key (for information retrieval functionality)

2. Clone the Repository
git clone [https://github.com/your-username/geolens.git](https://github.com/your-username/geolens.git)
cd geolens

3. Environment Setup
Create and activate a virtual environment:

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

Install the required Python dependencies:

pip install -r requirements.txt

(Note: You will need to create a requirements.txt file listing all your Python dependencies: Flask, tensorflow, keras, pandas, numpy, scikit-learn, etc.)

4. Configuration
Create a file named .env in the root directory and add your API key:

# .env file
SERPAPI_KEY="YOUR_SERPAPI_KEY_HERE"

5. Running the Application
The application is run via the Flask backend:

python app.py

The web dashboard will be available at http://127.0.0.1:5000.

📊 Key Performance Indicators (KPIs)
Our project success is measured against the following metrics:

Metric

Target

Rationale

Model Accuracy

≥90%


Ensures reliable classification for decision-making.

F1-Score

≥0.85


Confirms a strong balance between precision and recall, especially for rare classes.

Prediction Time

≤2
 seconds

Guarantees a fast user experience in the web application.

System Uptime

≥95%


Essential for continuous environmental monitoring reliability.

🤝 Team Members
This project was developed by the following team:

Name

Role

Responsibilities

Mohamed Ayman Fathy

Data Analyst

EDA, Visualization, Data Preprocessing, Oversight.

Mohamed Mourad

Data Scientist

Data Preprocessing, CNN model training & tuning.

Youssef Adawy

AI Engineer

Research validation, Model accuracy evaluation.

Mahmoud Mohamed Mahmoud

Web Developer

Flask backend integration, API deployment.

🗓️ Project Timeline (Key Milestones)
Milestone

Deliverable

Deadline

M1

Dataset Prepared and Preprocessed

9/15/2025

M2

Baseline CNN Model Trained & Evaluated

10/15/2025

M3

Advanced U-Net Model Implementation

10/30/2025

M4

Time-Series Forecasting Model Implemented

11/10/2025

M5

Flask App Integrated with Model & Dashboard Prototype

11/15/2025

M6

Final Report, Presentation & Full System Testing

11/20/2025
