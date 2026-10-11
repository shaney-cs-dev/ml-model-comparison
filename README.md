# ml-model-comparison
Machine Learning Model Comparison: Random Forest vs. XGBoost
# Machine Learning Model Comparison: Random Forest vs. XGBoost

## 📌 Project Overview
This project explores the use of machine learning models to predict a binary classification target.  
We implemented and compared **Random Forest** and **XGBoost** classifiers, tuning hyperparameters through cross‑validation and evaluating performance on unseen test data.

---

## ⚙️ Workflow
1. **Data Preparation**
   - Split dataset into training and test sets.
   - Applied preprocessing steps to ensure clean input features.

2. **Model Training**
   - **Random Forest**: Tuned hyperparameters using GridSearchCV.
   - **XGBoost**: Tuned hyperparameters (`max_depth`, `min_child_weight`, `learning_rate`, `n_estimators`) with GridSearchCV.

3. **Evaluation**
   - Used multiple metrics: **Precision, Recall, F1 Score, Accuracy**.
   - Created helper functions:
     - `get_test_scores()` → outputs test set performance in a clean table.
     - `make_results()` → summarizes cross‑validation results.

4. **Feature Importance**
   - Extracted and visualized feature importances from the best XGBoost model.
   - Identified top predictors driving model performance.

---

## 📊 Results
- **Random Forest**: Achieved acceptable performance (F1 ≥ 0.65 threshold).  
- **XGBoost**: Outperformed Random Forest on F1 score, showing better balance between precision and recall.  
- **Conclusion**: XGBoost is recommended as the final model due to stronger generalization and predictive power.

---

## 🔎 Insights
- The models highlight which features are most influential in predicting the target.
- While performance is solid, additional **feature engineering** (interaction terms, time‑based features, external contextual data) could further improve results.
- Even if predictive power is limited, the analysis provides valuable insights into the dataset and informs stakeholders about what drives outcomes.

---

## 🚀 Next Steps
- Deploy the tuned XGBoost model for production use.
- Explore new features and external data sources to enhance predictive performance.
- Document findings for stakeholders in both technical and business‑friendly formats.

---
