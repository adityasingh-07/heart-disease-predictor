# heart-disease-predictor
Predicting heart disease risk from clinical data, from EDA to a deployed, explainable ML app (scikit-learn · FastAPI · Streamlit · Docker).

**Work in progress** — currently in the data exploration phase.

An end-to-end machine learning project that predicts the risk of heart disease from clinical measurements, explains each prediction, and serves it through a web app.

**⚠️ Disclaimer:** This is an educational project. It is not a medical tool and must not be used for diagnosis.

## Goals

- Build and compare classification models using proper validation (no data leakage)
- Prioritise **recall** over raw accuracy, since missing a real case is worse than a false alarm
- Explain individual predictions with SHAP
- Serve the model through a REST API (FastAPI) with a Streamlit frontend
- Containerise with Docker and deploy

## Dataset

[UCI Heart Disease – Cleveland subset](https://archive.ics.uci.edu/dataset/45/heart+disease): 303 patients, 13 clinical features (e.g. age, cholesterol, chest pain type, max heart rate), and a binary target.

## Project structure

​```
├── data/        # Raw and processed data
├── notebooks/   # Exploratory analysis
├── src/         # Training and preprocessing code
├── api/         # FastAPI backend
├── app/         # Streamlit frontend
├── tests/       # Unit tests
└── models/      # Saved model artifacts
​```

## Roadmap

- [x] Project setup
- [ ] Exploratory data analysis
- [ ] Model training and evaluation
- [ ] Model explainability (SHAP)
- [ ] FastAPI backend
- [ ] Streamlit frontend
- [ ] Docker and deployment

## Running locally

​```bash
git clone https://github.com/<your-username>/heart-disease-predictor.git
cd heart-disease-predictor
python -m venv venv
source venv/bin/activate      # Windows: venv\Scripts\activate
pip install -r requirements.txt
​```

## Tech stack

Python · pandas · scikit-learn · matplotlib/seaborn · *(coming: SHAP, FastAPI, Streamlit, Docker)*
