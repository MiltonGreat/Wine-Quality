# Wine Quality Prediction

This project uses the **Wine Quality Dataset** to predict the quality of wines based on physicochemical features. The dataset is related to red variants of the Portuguese "Vinho Verde" wine and includes information about the chemical composition of the wine and how it relates to its quality. The main goal is to predict wine quality, which is given as an ordered integer score between 0 and 10.

### Dataset Overview

The Wine Quality Dataset contains the following attributes:

**Input Features:**
- `fixed acidity`: Acid content in wine
- `volatile acidity`: The amount of acetic acid in wine, which affects its taste
- `citric acid`: A component that contributes to wine's acidity
- `residual sugar`: The amount of sugar left after fermentation
- `chlorides`: Salt content in wine
- `free sulfur dioxide`: Amount of free sulfur dioxide
- `total sulfur dioxide`: Total sulfur dioxide in wine
- `density`: Density of the wine (density of water = 1)
- `pH`: pH level of the wine
- `sulphates`: Sulphate content, contributes to wine's aroma
- `alcohol`: Alcohol content in the wine

**Output Variable:**
- `quality`: The quality score of the wine (ranging from 0 to 10)

### Project Objective

The goal of this project is to:
- **Analyze** the features of wine and understand the relationship between them and wine quality.
- **Preprocess** the data by cleaning, normalizing numerical features, and applying one-hot encoding if necessary.
- **Build** a predictive model to classify wine quality based on the given features.
- **Evaluate** the performance of the model using classification metrics such as accuracy, confusion matrix, and classification report.

### Key Steps

1. **Data Preprocessing**
   - Handle missing values (if any).
   - Normalize numerical features using Min-Max scaling.
   - One-hot encode categorical features (if any).
   - Drop irrelevant or redundant columns.

2. **Exploratory Data Analysis (EDA)**
   - Visualize the distribution of the `quality` variable.
   - Explore relationships between different features using scatter plots and correlation matrices.

3. **Model Building**
   - Split the data into training and testing sets.
   - Apply **Logistic Regression** (or other models like Decision Trees, Random Forest, etc.).
   - Evaluate the model’s performance using metrics like accuracy, confusion matrix, and classification report.

4. **Model Evaluation**
   - Analyze the classification performance, including precision, recall, and F1-score.
   - Handle class imbalances (if needed).

### Source

https://www.kaggle.com/datasets/yasserh/wine-quality-dataset
