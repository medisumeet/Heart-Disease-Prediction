# ❤️ Heart Disease Prediction using Machine Learning & Deep Learning

## 📖 Project Overview

Heart disease is one of the leading causes of mortality worldwide. Early prediction can assist healthcare professionals in identifying high-risk patients and enabling timely medical intervention.

This project presents an end-to-end machine learning workflow for predicting heart disease using patient clinical data. The project includes Exploratory Data Analysis (EDA), statistical hypothesis testing, preprocessing, machine learning model development, hyperparameter tuning, and an Artificial Neural Network (ANN) for performance comparison.

---

# 🎯 Objectives

- Perform detailed exploratory data analysis.
- Identify significant clinical factors associated with heart disease.
- Validate feature relationships using statistical tests.
- Build reproducible preprocessing pipelines.
- Compare multiple machine learning algorithms.
- Develop an ANN model for comparison.
- Select the best-performing model using multiple evaluation metrics.

---

# 📂 Dataset

The dataset contains patient medical records with attributes such as:

- Age
- Sex
- Chest Pain Type
- Resting Blood Pressure
- Cholesterol
- Fasting Blood Sugar (FBS)
- Resting ECG
- Maximum Heart Rate (Thalach)
- Exercise Induced Angina
- Oldpeak
- ST Slope
- Number of Major Vessels
- Thalassemia
- Target (Heart Disease)

---

# 🔬 Methodology

## 1. Data Understanding

- Loaded and explored the dataset.
- Examined feature distributions.
- Checked data types and statistical summaries.
- Verified missing values and duplicate records.
- Analyzed class balance before model training.

---

## 2. Exploratory Data Analysis

EDA was performed to understand both univariate and multivariate relationships within the dataset.

The analysis included:

- Target distribution
- Gender-wise disease distribution
- Numerical feature distributions
- Correlation analysis
- Chi-Square hypothesis testing
- Cramer's V association analysis
- Relationship between categorical variables and target

---

## 3. Statistical Analysis

To validate feature significance, statistical tests were performed.

- Chi-Square Test
- Cramer's V Test

These tests helped distinguish statistically significant predictors from weakly associated variables.

---

## 4. Data Preprocessing

The preprocessing pipeline consisted of:

- Train-Test Split
- One-Hot Encoding
- Feature Scaling
- ColumnTransformer
- Scikit-learn Pipeline

The preprocessing workflow ensured consistency across all machine learning models.

---

## 5. Model Development

The following classification algorithms were implemented:

- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors
- Support Vector Machine
- Gaussian Naive Bayes
- Gradient Boosting
- AdaBoost
- Artificial Neural Network (ANN)

---

## 6. Hyperparameter Tuning

GridSearchCV was used to optimize selected models and improve predictive performance.

---

# 📊 Exploratory Data Analysis Findings

The EDA revealed several meaningful insights about the dataset.

### Target Distribution

- The target variable is **reasonably balanced**, making the dataset suitable for supervised classification without requiring extensive resampling techniques.

### Gender Analysis

- **Male patients are more prone to heart disease** than female patients according to the observed distribution.

### Fasting Blood Sugar (FBS)

- Chi-Square analysis indicates **no statistically significant relationship** between Fasting Blood Sugar (FBS) and heart disease.

### Cholesterol

- Statistical testing suggests **no significant association between FBS and cholesterol levels**.

### Resting ECG

- Chi-Square testing found a **significant association between Resting ECG and heart disease**.
- Cramer's V analysis indicates that this association is **strong enough to contribute to prediction**.

### Maximum Heart Rate (Thalach)

- A **moderate positive relationship** exists between Maximum Heart Rate (Thalach) and the target variable.
- Patients with higher Thalach values were more likely to belong to the positive heart disease class in this dataset.

---

# 🤖 Model Performance

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|--------|---------:|----------:|--------:|---------:|---------:|
| **Naive Bayes** | **85.25%** | **85.29%** | **87.88%** | **86.57%** | **0.912** |
| Logistic Regression | 85.25% | 87.50% | 84.85% | 86.15% | 0.906 |
| Random Forest | 81.97% | 86.67% | 78.79% | 82.54% | 0.895 |
| AdaBoost | 81.97% | 86.67% | 78.79% | 82.54% | 0.893 |
| Artificial Neural Network | 81.97% | 82.35% | 84.85% | 83.58% | 0.877 |
| SVM | 80.33% | 86.21% | 75.76% | 80.65% | 0.878 |
| KNN | 80.33% | 86.21% | 75.76% | 80.65% | 0.861 |
| Gradient Boosting | 77.05% | 80.65% | 75.76% | 78.13% | 0.854 |
| Decision Tree | 65.57% | 67.65% | 69.70% | 68.66% | 0.652 |

---

# 📌 Key Findings

- The dataset is sufficiently balanced, making it appropriate for classification without additional balancing techniques.
- Male patients exhibited a higher prevalence of heart disease than female patients.
- Fasting Blood Sugar (FBS) showed **no statistically significant relationship** with heart disease.
- Resting ECG demonstrated a statistically significant association with the target variable.
- Maximum Heart Rate (Thalach) showed a moderate positive relationship with heart disease occurrence.
- Among all evaluated models, **Gaussian Naive Bayes achieved the highest ROC-AUC (0.912)** while also obtaining one of the highest accuracies (**85.25%**).
- Logistic Regression achieved the same overall accuracy as Naive Bayes with slightly higher precision but lower recall.
- Ensemble models such as Random Forest and AdaBoost provided stable performance but did not outperform Naive Bayes on this dataset.
- The ANN achieved competitive performance (81.97% accuracy), indicating that traditional machine learning models were better suited for this structured dataset.

---

# 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

---

# 📁 Project Structure

```
Heart-Disease-Prediction/
│
├── EDA.ipynb
├── Model_Building.ipynb
```

---

# 💡 Conclusion

This project demonstrates a complete machine learning workflow for heart disease prediction by integrating exploratory data analysis, statistical hypothesis testing, classical machine learning algorithms, and deep learning techniques.

The results indicate that **Gaussian Naive Bayes and Logistic Regression outperformed more complex ensemble methods** on this dataset, suggesting that simpler probabilistic and linear models can be highly effective for structured clinical data. Additionally, statistical analysis highlighted the importance of features such as Resting ECG and Maximum Heart Rate, while showing that Fasting Blood Sugar was not a significant predictor.

---

## 👨‍💻 Author

**Medi Sumeet**

- GitHub: [Github](https://github.com/medisumeet)
- LinkedIn: [LinkedIn](https://www.linkedin.com/in/medi-sumeet-5b8a6631b/)
