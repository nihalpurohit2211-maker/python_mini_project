# python_mini_project
it is a machine learning python mini project

# 📉 Machine Learning Pipeline: Predicting Layoff Risk

## 📌 Project Overview
This project involves building an end-to-end Machine Learning classification pipeline to predict an employee's likelihood of facing workforce displacement. By analyzing job characteristics, skill requirements, and AI adoption factors, this model classifies employees into three risk categories: **Low, Medium, and High**.

## 📊 Dataset
* **File:** `ai-impact-jobs-layoff-risk-dataset.csv`
* **Size:** 20,000 records, 16 features.
* **Features Used:** Age, Education Level, Years of Experience, Industry, Job Role, Company Size, AI Adoption Level, Tasks Automated Percentage, and more.
* **Target Variable:** `Layoff_Risk` (Classification)

## ⚙️ The Machine Learning Pipeline
This project follows a structured data science workflow:
1. **Exploratory Data Analysis (EDA):** Investigated data distributions, checked for missing values/duplicates, and visualized relationships (e.g., Layoff Risk vs. Industry).
2. **Data Preprocessing:** * Handled extreme outliers in numerical data using the **IQR method**.
   * Encoded categorical text variables into machine-readable numeric formats using **One-Hot Encoding** (`pd.get_dummies`).
   * Encoded the target variable using `LabelEncoder`.
3. **Data Splitting & Scaling:** Split the dataset into 80% training and 20% testing sets. Applied `StandardScaler` to ensure numerical features were weighted equally.
4. **Model Training:** Trained two distinct classification models:
   * **Logistic Regression** * **Random Forest Classifier**
5. **Evaluation:** Compared models using Accuracy Scores, Confusion Matrix heatmaps, and extracted Feature Importance.

## 🏆 Results & Conclusion
After evaluating both models on the test data:
* **Logistic Regression Accuracy:** [0.9401]
* **Random Forest Accuracy:** [0.8745]

**Winning Model:** The [Logistic Regression Accuracy] performed the best on this dataset. 



## 🚀 How to Run this Project
1. Clone this repository or download the files.
2. Ensure you have Python installed along with the following libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn`.
3. Open `mini_project.ipynb` in Google Colab or Jupyter Notebook.
4. Ensure the dataset CSV is in the same directory.
5. Select "Run All" to execute the pipeline.
