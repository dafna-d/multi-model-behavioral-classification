# Predictive Behavioral Analytics & Classification Engine 

## 📌 Executive Summary
In clinical research and behavioral economics, accurately identifying risk factors for substance dependency requires scalable, data-driven approaches. 

This project implements an enterprise-grade Machine Learning pipeline that translates complex psychological profiles (e.g., Neuroticism, Extraversion) and demographic metadata into actionable predictive insights. The system was architected to handle real-world data challenges, specifically focusing on imbalanced classification, feature engineering, and decision-threshold optimization to maximize predictive reliability.


##  Architecture & Methodology
* **Data Engineering Pipeline:** Engineered a robust preprocessing workflow including automated cleaning of noisy data, custom categorical mapping, One-Hot Encoding, and strict feature scaling (`StandardScaler`) to prepare the data for distance-based and linear algorithms.
* **Algorithmic Strategy & Benchmarking:** Developed and evaluated a suite of machine learning models to solve for complex relationships in the data:
  * **Logistic Regression (Optimized):** Implemented `LogisticRegressionCV` with dynamic regularization. Engineered the decision boundary using the ROC curve and Youden's J statistic to find the optimal probability threshold, minimizing critical errors in an imbalanced dataset.
  * **Random Forest Classifier:** Leveraged ensemble methods (100 estimators) with class-weight balancing to ensure stable, robust predictions across minority classes.
  * **Decision Tree & KNN:** Deployed as baseline architectures to evaluate depth complexity and spatial clustering.
* **Model Interpretability:** Extracted feature importance and logistic coefficients to provide stakeholders with clear, explainable AI insights regarding which specific traits drive behavioral risks.

 <img width="1256" height="690" alt="צילום מסך 2026-09-07 102521" src="https://github.com/user-attachments/assets/cd432ed5-5ae9-4010-861b-df3eab3bda1c" />


##  Key Business & Clinical Insights
* **Actionable Intelligence:** Demonstrated how statistical correlations can be transformed into a predictive engine, providing a data foundation for targeted behavioral interventions.
* **Advanced Metrics Focus:** Showcased a deep understanding of business logic by prioritizing the F1-score and Recall over standard Accuracy, reflecting the real-world cost of false negatives in risk prediction.

##  Tech Stack & Tooling
* **Core Environment:** Python 3.x, Jupyter Notebooks
* **Data Engineering & EDA:** `pandas`, `numpy`
* **Machine Learning:** `scikit-learn` (Classification, Cross-Validation, Metrics, Preprocessing)
* **Data Visualization:** `matplotlib`, `seaborn`

## 📂 Repository Structure
* `ML-project-Substance-use-prediction-model.ipynb`: The core analytical engine and modeling pipeline.
* `Presentation.pdf`: Executive deck detailing methodology, model selection, and final insights.
* `requirements.txt`: Environment dependencies.

## ⚙️ Deployment Instructions
Clone the repository and install the required dependencies to run the predictive engine locally:
```bash
pip install -r requirements.txt
