# 🧠 Obesity Prediction

A machine learning project that predicts an individual's **obesity level** based on various health, lifestyle, and demographic features.  
The project includes complete data preprocessing, model training, evaluation, and prediction steps — all implemented in a Jupyter Notebook.

---

## 📌 Overview

Obesity is one of the most pressing health challenges worldwide. This project aims to build a **classification model** capable of predicting obesity levels using supervised learning techniques.  
The workflow includes **data cleaning, feature engineering, model selection, and evaluation** to identify the best-performing algorithm.

---

## 📂 Repository Structure

ObesityPrediction/
│
├── ProjectFile.ipynb # Main Jupyter Notebook (data analysis, model training, evaluation)
├── ProjectReport.pdf # Report with explanation, methodology, and findings
├── train.csv # Training dataset with labeled samples
├── test.csv # Test dataset for evaluation or submission
├── BestSolution.csv # Output file containing predictions from the best model
└── README.md # This file


---

## 🧬 Dataset Description

The dataset contains health, lifestyle, and demographic information.  
Each row represents one individual with features like:

| Feature | Description |
|----------|-------------|
| Gender | Male / Female |
| Age | Age in years |
| Height | Height in meters |
| Weight | Weight in kilograms |
| Family History | Family obesity history (Yes/No) |
| Physical Activity | Daily/weekly activity level |
| Daily Meals | Number of meals per day |
| Caloric Intake | Level of calorie consumption |
| Transportation Mode | How the individual commutes (e.g., walking, car, bike) |
| **Target Variable** | Obesity level (Underweight, Normal, Overweight, Obesity) |

*(Modify this table if your dataset has slightly different columns.)*

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Load and inspect datasets (`train.csv`, `test.csv`)
- Handle missing values
- Encode categorical variables using LabelEncoder or One-Hot Encoding
- Normalize/scale numeric features (e.g., MinMaxScaler)
- Perform feature engineering (e.g., BMI calculation if applicable)

### 2. Exploratory Data Analysis (EDA)
- Analyze feature distributions and correlations
- Visualize with **Matplotlib** and **Seaborn**
- Identify class imbalance (if any)

### 3. Model Training
Several machine learning algorithms were trained and compared:
- Logistic Regression  
- Decision Tree Classifier  
- Random Forest Classifier  
- XGBoost / Gradient Boosting  

Model selection was based on validation accuracy, precision, recall, and F1-score.

### 4. Hyperparameter Tuning
- Used GridSearchCV or RandomizedSearchCV to find optimal parameters
- Evaluated models using cross-validation (e.g., k=5)

### 5. Model Evaluation
- Calculated metrics:
  - **Accuracy**
  - **Precision**
  - **Recall**
  - **F1-score**
  - **Confusion Matrix**
- Chose the model with the best balance between performance and interpretability

### 6. Final Prediction
- Applied the best model to `test.csv`
- Generated predicted obesity levels
- Saved results in `BestSolution.csv`

---

## 📊 Results & Insights

- The best-performing model achieved **high accuracy** on validation data.
- **Feature importance analysis** showed that factors such as BMI, physical activity, and eating habits had the highest influence on predictions.
- Visualization and metrics confirmed good generalization performance.

*(You can update this section with actual numeric results once finalized.)*

---

## 🧰 Technologies Used

| Category | Tools / Libraries |
|-----------|------------------|
| Programming Language | Python |
| Data Processing | pandas, numpy |
| Visualization | matplotlib, seaborn |
| Machine Learning | scikit-learn, xgboost |
| Development | Jupyter Notebook |

---

