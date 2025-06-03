
# 🫀 Heart Failure Prediction using Machine Learning

## 📌 Overview

This project uses various supervised machine learning models to predict heart disease from clinical features. Through exploratory data analysis and classification models, the aim is to assist in early detection of cardiovascular risk.

## 📊 Dataset

- The dataset contains **clinical records** of patients such as:
  - Age, Sex, Chest Pain Type
  - Resting Blood Pressure, Cholesterol
  - Fasting Blood Sugar, Resting ECG, Exercise Angina
  - Oldpeak, ST Slope, Max Heart Rate
- **Target Variable**: `HeartDisease` (0 = No, 1 = Yes)

## 🔍 Exploratory Data Analysis (EDA)

Performed visual analysis of key features:
- Countplots of categorical features like `Sex`, `ChestPainType`, `RestingECG`, `ExerciseAngina`, and `ST_Slope`
- Pie charts to compare distributions between patients **with and without heart disease**
- Histograms and boxplots to analyze numeric features like `Cholesterol`, `Age`, `RestingBP`, `MaxHR`, etc.

## 🧹 Data Preprocessing

- Categorical encoding using `LabelEncoder` and `get_dummies`
- Feature scaling using `StandardScaler`
- Split data into training and testing sets using `train_test_split`

## 🧠 Machine Learning Models Applied

Implemented and compared the performance of multiple ML models:

| Model                  | Library Used        |
|-----------------------|---------------------|
| Logistic Regression   | `sklearn.linear_model` |
| K-Nearest Neighbors   | `sklearn.neighbors` |
| Decision Tree         | `sklearn.tree`      |
| Random Forest         | `sklearn.ensemble`  |
| Gaussian Naive Bayes  | `sklearn.naive_bayes` |
| Support Vector Classifier | `sklearn.svm`   |
| LightGBM              | `lightgbm`          |

## 📈 Evaluation Metrics

For each model, the following metrics were computed:
- Accuracy
- Confusion Matrix
- Classification Report (Precision, Recall, F1-score)
- ROC Curve and AUC Score

## 🏆 Best Performing Model

- **[Insert Best Model Name Here]**
- Achieved highest accuracy and balanced performance on the test set.

## 📌 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/heart-failure-prediction.git
   cd heart-failure-prediction
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook:
   ```bash
   jupyter notebook Heart-Failure-Prediction.ipynb
   ```

## 🧠 Future Work

- Hyperparameter tuning with `GridSearchCV`
- Deploy as a web app using Flask or Streamlit
- Integrate patient-specific recommendations

## ⚖️ Disclaimer

This project is for **educational purposes only**. It is not intended for use in actual medical diagnosis or treatment.
