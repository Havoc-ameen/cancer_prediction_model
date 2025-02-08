# cancer_prediction_model
📊 Exploring cancer data through regression models, this project utilizes machine learning to analyze outcomes and develop predictive models for deeper insights.

# 🏥 Cancer Regression Analysis

## 📌 Project Overview
This project aims to predict cancer-related outcomes using various regression models. It involves data preprocessing, feature engineering, and model evaluation to identify the most effective regression approach for accurate predictions.

## 🔬 Key Techniques Used:
- 📂 **Data Cleaning & Processing**: Handling missing values, encoding categorical variables.
- 🏗️ **Feature Engineering**: Transformation and scaling techniques.
- 📊 **Exploratory Data Analysis (EDA)**: Understanding data distributions and relationships.
- 🤖 **Multiple Regression Models**: Evaluating linear and non-linear regression techniques.
- 🔄 **Regularization Techniques**: Lasso, Ridge, and Elastic Net to prevent overfitting.
- 📈 **Model Evaluation Metrics**: MSE, RMSE, MAE, and R² score.

## 📊 Dataset Description
The dataset contains multiple features related to cancer diagnostics, used to predict a key target variable.

### Key Data Processing Steps:
- 🛠️ **Handling Missing Values**: Using median imputation.
- 🔤 **Feature Encoding**: Transforming categorical variables.
- 📏 **Scaling & Normalization**: Standardizing the dataset for better model performance.
- ⚠️ **Outlier Treatment**: Applied IQR-based Winsorization.

## 📈 Regression Models & Performance
The following regression models were implemented and evaluated:

### 1️⃣ Polynomial Regression
- Captures non-linear relationships between features.
- **Challenges**: Overfitting and instability in predictions.

### 2️⃣ Regularized Regression Models
To reduce overfitting, Lasso, Ridge, and Elastic Net regression were applied:

| Model                  | Training Accuracy | Testing Accuracy |
|------------------------|------------------|------------------|
| Lasso Regression      | 54.23%           | 53.48%           |
| Ridge Regression      | 54.82%           | 53.35%           |
| Elastic Net Regression | 54.38%           | 53.54%           |

### 3️⃣ Tree-Based & Non-Linear Models
Additional models were tested for performance improvements:

| Model                    | Training Accuracy | Testing Accuracy |
|--------------------------|------------------|------------------|
| K-Nearest Neighbors (KNN) | 42.07%           | 6.67%            |
| Support Vector Regression | 20.36%           | 21.70%           |
| Decision Tree Regression  | 99.90%           | 12.87%           |
| Random Forest Regression  | 93.42%           | 57.19%           |

### 🔎 Observations:
- 🌳 **Tree-based models** (Decision Tree, Random Forest) show high variance and tend to overfit.
- 📉 **Regularized regression models** (Lasso & Ridge) strike a balance between bias and variance.
- ⚙️ **SVR and KNN** exhibit sensitivity to hyperparameter tuning.

## 🚀 Installation & Usage

### 📌 Prerequisites:
Ensure you have Python 3.x installed with the required dependencies.

### 📦 Install Required Libraries:
```bash
pip install pandas numpy matplotlib scikit-learn
```
## 🔧 Running the Project:
### 1. Clone the repository: 
``` bash
git clone https://github.com/Havoc-ameen/cancer_prediction_model
```
 ### 2. Navigate to the project folder: 
``` bash
cd cancer-regression
```
 ### 3. Open and run the Jupyter Notebook: 
``` bash
jupyter notebook "Cancer_Regression.ipynb"
```

## 📌 Key Takeaways:
- ⚠️ Polynomial Regression lacks stability and generalization.
- 📉 Lasso and Ridge Regression provide a good balance between bias and variance.
- 🌲 Random Forest and Decision Trees overfit easily—pruning or hyperparameter tuning is necessary.
- 🏗️ Feature selection and scaling have a significant impact on model performance.
## 🐝 License
- This project is licensed under the MIT License.
