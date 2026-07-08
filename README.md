# NEO Hazard Predictor

A machine learning project that classifies near-Earth asteroids as hazardous or not hazardous, using NASA's Near-Earth Object dataset.

Live app: https://huggingface.co/spaces/Rozina66/neo-hazard-predictor6

Overview

This project covers the full pipeline from raw data to a deployed, interactive application:


Exploratory data analysis — class distribution, feature distributions, and correlation analysis
Baseline model — Logistic Regression
Neural network model — Multi-Layer Perceptron (MLP)
XGBoost model — tuned using GridSearchCV and evaluated with ROC-AUC
Model explainability — SHAP global feature importance, beeswarm plots, force plots, and dependence plots
Deployment — the final model deployed as an interactive web application on Hugging Face Spaces


The goal was to build a model that is both accurate and interpretable, and to take it beyond the notebook stage into a usable, deployed application.

Features used


Estimated minimum diameter (km)
Estimated maximum diameter (km)
Relative velocity (km/h)
Miss distance (km)
Absolute magnitude (H)


Project structure

neo-hazard-predictor/
├── README.md
├── notebook/
│   └── NEO_Hazard_Predictor.ipynb
├── app/
│   ├── app.py
│   ├── model.pkl
│   ├── scaler.pkl
│   └── requirements.txt

Running locally

pip install -r app/requirements.txt
python app/app.py

Tech stack

Python, scikit-learn, XGBoost, SHAP, Gradio, pandas, NumPy

Screenshots
<img width="3866" height="768" alt="neo_predictor_linkedin" src="https://github.com/user-attachments/assets/2eb672a3-f901-493d-8e51-f299d573db42" />

Not hazardous result and hazardous result shown side by side below.
