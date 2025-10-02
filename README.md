# trade-anomaly-detection-dashboard
An ML + AI system for detecting anomalies in global trade data with an interactive dashboard.

# 🌍 Trade Anomaly Detection Dashboard

A machine learning + AI system to **detect anomalies in global trade flows**, enriched with **sanctions, shipping, and economic signals**, and visualized in an **interactive dashboard**.

This project demonstrates end-to-end data science/ML workflow:
- Large-scale data ingestion (UN Comtrade, sanctions lists, shipping data, news sentiment).
- Cleaning & feature engineering with Spark/Dask.
- Anomaly detection using statistical, ML, and deep learning models.
- Deployment of models via FastAPI + Docker.
- Interactive Streamlit dashboard for exploration and storytelling.

---

## 🚀 Features

- **Data Pipeline**: Automated ingestion from multiple sources (trade, sanctions, shipping, news).
- **ML/AI Models**: Classical (Isolation Forest, One-Class SVM), ML (XGBoost/LightGBM), Deep Learning (LSTM/Transformers).
- **Contextual Layers**: Sanctions overlays, tariff schedules, macroeconomic indicators, and news sentiment analysis.
- **Dashboard**: Interactive world map + time-series anomaly explorer with sanctions/events timeline.
- **Cloud-Ready**: Optional deployment with AWS S3 + SageMaker, but free/open-source by default.
- **Version Control & Reproducibility**: GitHub for code, MLflow for experiments.

---

## 📊 Architecture

![Architecture Diagram](docs/architecture_diagram.png)

**Pipeline Flow:**
1. **Ingestion** → APIs (UN Comtrade, WTO, OFAC, UNCTAD, GDELT) → Raw storage (CSV/Parquet, optional S3).
2. **Processing** → Dask/Spark + Pandas → Clean + Feature Engineering.
3. **Modeling** → ML/AI models → Anomaly Scores.
4. **Deployment** → FastAPI service + Docker.
5. **Visualization** → Streamlit dashboard with maps + timelines.

---

## 📂 Repository Structure

