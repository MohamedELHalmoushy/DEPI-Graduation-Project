# 🌍 Land Classification – DEPI Graduation Project

## 📌 Overview
This repository contains my **DEPI Graduation Project**, which focuses on **Land Classification using Remote Sensing data**.  
The project covers the full pipeline from data loading and preprocessing to Exploratory Data Analysis (EDA), model development, evaluation, and documentation.

It demonstrates the use of **NDVI, RGB, and RGB+NIR composite imagery** for building land-classification models and comparing their performance across different preprocessing and feature-extraction workflows.

---

## 🚀 Project Objectives
- Load and preprocess remote-sensing datasets  
- Perform detailed **Exploratory Data Analysis (EDA)**  
- Build multiple classification models:
  - NDVI-based classification
  - RGB classification
  - RGB + NIR classification
- Evaluate and compare models
- Document system design using UML (Activity, State, Sequence, Use-Case diagrams)
- Present the work in a structured and professional graduation report

---

## 📂 Repository Structure
DEPI-Graduation-Project/
│
├── Loading_Data&EDA_Final.ipynb
├── NDVI_model.ipynb
├── RGB_model.ipynb
├── RGB_NIR.ipynb
├── scraper.ipynb
│
├── Activity Diagram.pdf
├── Sequence Diagram.pdf
├── State Diagram.pdf
├── Use case diagram.pdf
│
├── Documentation_DEPI_PROJECT_Mohamed_Ayman_LAND_CLASSIFCATION_1.pdf
├── Land Classification.pptx
│
├── LICENSE
└── README.md

## 🧪 Technologies & Tools

| Category | Tools |
|----------|-------|
| Languages | Python |
| Libraries | NumPy, Pandas, Matplotlib, Rasterio, scikit-learn |
| Visualization | Matplotlib, Seaborn |
| Remote Sensing Metrics | NDVI, RGB Composite, NIR |
| Documentation | UML Diagrams, PDF Report, PowerPoint |

---

## 🛠️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/MohamedELHalmoushy/DEPI-Graduation-Project.git
cd DEPI-Graduation-Project
```

  install_dependencies:
    description: "Install required Python libraries"
    commands:
      - "pip install numpy pandas matplotlib scikit-learn rasterio"

usage:
  preprocessing_and_eda:
    description: "Run preprocessing and exploratory data analysis"
    open_notebook: "Loading_Data&EDA_Final.ipynb"

  train_models:
    description: "Choose and run any model notebook"
    notebooks:
      - name: "NDVI_model.ipynb"
        description: "NDVI-based classifier"
      - name: "RGB_model.ipynb"
        description: "RGB-based classifier"
      - name: "RGB_NIR.ipynb"
        description: "RGB + NIR classifier"

    each_notebook_includes:
      - "Data loading"
      - "Feature extraction"
      - "Model training"
      - "Evaluation metrics"
      - "Visualizations"

documentation:
  included_files:
    - "Full Project Report (PDF)"
    - "Activity Diagram (PDF)"
    - "Sequence Diagram (PDF)"
    - "State Diagram (PDF)"
    - "Use Case Diagram (PDF)"
    - "Final Presentation (PPTX)"

author:
  name: "Mohamed Ayman"
  role: "DEPI Student — Land Classification Project"
  github: "https://github.com/MohamedELHalmoushy"

license:
  type: "MIT License"
  description: "This project is licensed under the MIT License."
