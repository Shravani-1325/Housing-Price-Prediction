# 🏡 Housing Price Prediction - Binary Classifier on Structured Dataset

## 📋 Project Overview
This project focuses on predicting housing prices in India using a structured dataset. By leveraging advanced machine learning algorithms, we aim to create an accurate binary classification model.

## 🌟 Objectives
- Understand and implement EDA for structured datasets.
- Build a predictive model for housing prices.
- Use CRISP-DM methodology for project structuring.
- Evaluate the model using key metrics like accuracy, precision, recall, and F1-score.

## 📂 Dataset Description
- **Source**: Kaggle - *House Prices India* dataset.
- **Size**: 23 columns, 14,619 rows.
- **Features**:
  - `number of bedrooms`, `number of bathrooms`, `living area`, `lot area`, etc.
  - Target: `Price`.

## 📊 Methodology - CRISP-DM
### 🔍 1. Business Understanding
The project aims to predict whether house prices are above or below 6 million INR using detailed residential property data.

### 📊 2. Data Understanding
- The dataset contains various features like the number of bedrooms, bathrooms, living area, and more.
- Used EDA to analyze and summarize the dataset.

### 🛠️ 3. Data Preparation
- **Cleaning**: Handled missing values and scaled numerical features.
- **Feature Engineering**: Created new attributes, such as:
  - `Age of the House` (2024 - Built Year).
  - `Total Area` (sum of living area and basement area).

### 🤖 4. Model Training
- Algorithms used:
  - Logistic Regression
  - Random Forest
- Trained the model with 50 epochs and optimized for accuracy and precision.

### 📈 5. Model Evaluation
- Metrics used:
  - Accuracy: 97%
  - Precision, Recall, F1-score
- Random Forest outperformed other models with an F1 score of 0.98.

### 📦 6. Deployment
- The model can classify whether a house price is above or below the threshold.

## 📊 Key Findings and Visualizations
### 1️⃣ Distribution of House Age
- Most houses are 20 years old, indicating a construction boom 20 years ago.

### 2️⃣ Average Price by Number of Bedrooms
- 8-bedroom houses have the highest average price due to the presence of luxury properties.
- Prices tend to drop for houses with more than 8 bedrooms due to lower demand and fewer samples.

### 3️⃣ Correlation Between Total Area and Price
- Larger houses (greater total area) tend to have higher prices due to increased desirability.

### 4️⃣ Feature Correlation with Price
- The `living area` has the strongest positive correlation with price, followed by `number of bathrooms` and `grade of the house`.

## 🏆 Results
- **Best Model**: Random Forest
  - **Accuracy**: 97%
  - **F1 Score**: 0.98
- **Confusion Matrix**:
  - True Positives (TP): 130
  - True Negatives (TN): 2706
  - False Positives (FP): 17
  - False Negatives (FN): 71

## 🚀 How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/housing-price-prediction.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the training script:
   ```bash
   python train.py
   ```

## 💡 Insights and Future Scope
- The model performs well but can be improved with:
  - Hyperparameter tuning.
  - Using ensemble methods.
  - Adding more features for better predictions.
- Future work includes deploying the model as a web app for real-time predictions.
