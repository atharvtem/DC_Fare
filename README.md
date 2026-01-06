# 🚕 DC Taxi Fare Prediction 

## 📌 Project Overview
This project analyzes and models taxi trip data collected by the District of Columbia government to predict **taxi fare amounts** using trip characteristics such as distance, duration, airport involvement, trip type, payment method, and temporal features.

The project follows a **complete data science lifecycle**, including:
- Data collection
- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Feature engineering
- Machine learning modeling
- Model evaluation and ethical reflection

---

## 📊 Dataset
- **Source:** DC Open Data – Taxicab Trip Records (2024)
- **Public Link:** https://dcgov.app.box.com/v/TaxiTrips2024
- **Size:** ~2.5 million records
- **Time Period:** January–December 2024
- **Granularity:** Block-level pickup and drop-off locations (no exact addresses)

> Due to dataset size and privacy considerations, the full dataset is **not included** in this repository.  
> A small sample is provided for testing and demonstration purposes.

---

## 🎯 Problem Statement
**Can we accurately predict taxi fare amounts based on trip features such as mileage, duration, airport involvement, trip type, and payment method?**

---

## 🧪 Methods & Techniques
- Data merging across monthly files
- Duplicate resolution using composite identifiers
- Missing value analysis and imputation
- Outlier detection (Z-score and IQR methods)
- Feature engineering (Haversine distance)
- Exploratory data visualization
- Sampling strategies for large-scale data
- Supervised regression modeling

---

## 🤖 Machine Learning Models
The following models were trained and evaluated:

- Linear Regression (baseline)
- Random Forest Regressor
- Gradient Boosting Regressor
- XGBoost Regressor
- Neural Network (MLP Regressor)

The **Neural Network (MLP)** achieved the best performance.

---

## 📈 Model Performance (Best Model – Neural Network)

| Metric | Value |
|------|------|
| R² Score | ~0.96 |
| MAE | ~1.19 |
| RMSE | ~2.36 |

Model performance improved significantly with increased sample size, highlighting the importance of **data quantity** for complex models.

---

## ⚖️ Ethical Considerations
- Privacy risks from location-based data (latitude/longitude)
- Fairness concerns in geographic modeling
- Responsible use of government-collected mobility data
- Transparency around modeling limitations (e.g., straight-line distance vs road distance)

---

## 🛠 Tech Stack
- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  
- Matplotlib, Seaborn  
- Google Colab  

---

## ▶️ How to Run the Project

### **Step 1: Clone the Repository**
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
