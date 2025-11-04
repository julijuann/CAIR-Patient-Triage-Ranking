# Patient Triage Ranking System

A Python-based machine learning project that uses NLP to process emergency room intake forms and rank patients by urgency. The goal is to support nurses by automatically prioritizing patients based on symptoms, medical history, and risk factors to reduce wait times and improve triage efficiency.

---

## Project Overview

* **NLP Pipeline**: Extracts key information (symptoms, medical history, vitals) from patient intake forms.
* **Machine Learning Model**: Trains on labeled data to predict urgency scores using supervised learning.
* **Ranking System**: Updates dynamically as new forms arrive, maintaining a real-time prioritized list.
* **Example**: A patient with *shortness of breath + asthma history* ranks higher than one with *shortness of breath* alone.

---

## Team Roles

**Project Lead - Julian**
Oversees development, defines workflow, and integrates components into a functioning prototype.

**NLP/Model Engineer**
Builds text preprocessing, entity extraction, and model training pipeline for urgency prediction.

**Data Engineer**
Manages data ingestion, cleaning, and feature extraction from structured and unstructured form data.

**Evaluation & UI Engineer**
Develops performance metrics, evaluation dashboards, and a simple interface for displaying ranked patients.

---

## Tech Stack

Python · pandas · scikit-learn · spaCy · XGBoost · FastAPI · Streamlit

---

## Structure
(simple outline of what our repo should look like)

```
patient-triage/
├── data/              # Intake form samples (de-identified)
├── src/
│   ├── nlp/           # Text preprocessing and entity extraction
│   ├── model/         # Training and inference scripts
│   ├── queue/         # Ranking and update logic
│   └── app/           # Streamlit/FastAPI interface
└── README.md
```

---

## Next Steps

1. Collect and clean sample triage form data (synthetic/de-identified).
2. Build NLP preprocessing and symptom-history mapping.
3. Train baseline model for urgency scoring.
4. Create live ranking dashboard to simulate patient intake flow.
