# Wine Quality 

### Overview

The dataset consists of 1,143 records of red wine with 11 input features and 1 target column indicating the wine quality. The features include physicochemical properties like acidity, alcohol content, pH, sulfur levels, and density. The quality column is rated on a scale from 3 to 8, where a higher number indicates better quality.

### Objectives 

This data science project designed to:

- Explore and analyze the physicochemical properties of wine.
- Build and evaluate machine learning models to classify wine quality.
- Use data preprocessing techniques to normalize features for better model performance.

### EDA Questions

I want to answer the following questions:

1. What is the distribution of wine quality ratings?
2. What are the relationships between the features?
3. What is the correlation between physicochemical properties?

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

### Features

- fixed acidity: Titrable acidity in wine (g tartaric acid per liter)
- volatile acidity: Amount of acetic acid in wine (g per liter)
- citric acid: Amount of citric acid (g per liter)
- residual sugar: Residual sugar content (g per liter)
- chlorides: Amount of chlorides (g per liter)
- free sulfur dioxide: Free sulfur dioxide content (ppm)
- total sulfur dioxide: Total sulfur dioxide content (ppm)
- density: Density of the wine (g/cm³)
- pH: pH of the wine
- sulphates: Sulphate content (g per liter)
- alcohol: Alcohol content (percentage)
- quality: Quality rating (3 to 8)
- Id: Unique identifier (not used for prediction)

### Key Steps

1. **Data Loading & Exploration**
- The dataset is loaded and initial exploration is done to check the data's structure, types, and basic statistics.

2. **Data Cleaning & Transformation**
- Missing values are handled by imputing with the median of each column.

3. **Feature Scaling**
- All the features are scaled using StandardScaler to normalize them for machine learning models.

4. **Dimensionality Reduction**
- PCA (Principal Component Analysis) is applied to reduce highly correlated features, retaining 95% of the variance.

5. **Class Imbalance Handling**
- SMOTE (Synthetic Minority Over-sampling Technique) is used to balance the distribution of wine quality ratings by generating synthetic samples for minority classes.

6. **Data Splitting**
- The dataset is split into training and testing sets (80% training, 20% testing).

7. **Visualization**
- Correlation heatmaps and distribution plots are created to visually understand the relationships between features and the target variable.

### Future Work

- Build and compare machine learning models such as Logistic Regression, Random Forest, and XGBoost.
- Experiment with hyperparameter tuning to improve model performance.
- Implement feature selection techniques to optimize the model.

### Source

Dataset: [Wine Quality Dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/wine-quality-dataset)
