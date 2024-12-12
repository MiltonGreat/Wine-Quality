# Wine Quality 

### Overview

This prepares data from the Wine Quality Dataset to predict the quality of wine based on its physicochemical attributes. The dataset is preprocessed and analyzed to gain insights. The data is prepared for the next step of choosing a machine learning model that can be applied to classify the quality of wine.

### Objectives 

This data science project designed to:

- Explore and analyze the physicochemical properties of wine.
- Build and evaluate machine learning models to classify wine quality.
- Use data preprocessing techniques to normalize features for better model performance.

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

### Key Steps

1. **Data Preprocessing**
   - Handle missing values (if any).
   - Normalize numerical features using Min-Max scaling.
   - One-hot encode categorical features (if any).
   - Drop irrelevant or redundant columns.

2. **Exploratory Data Analysis (EDA)**
   - Visualize the distribution of the `quality` variable.
   - Explore relationships between different features using scatter plots and correlation matrices.

### Visualizations

- Correlation Heatmap: Displays relationships between features.
- Feature Distributions: Understand the distribution of physicochemical properties.

### Future Work

- Build and compare machine learning models such as Logistic Regression, Random Forest, and XGBoost.
- Experiment with hyperparameter tuning to improve model performance.
- Implement feature selection techniques to optimize the model.
- Deploy the model using Streamlit or Flask for real-world usage.

### Source

https://www.kaggle.com/datasets/yasserh/wine-quality-dataset
