# Wine Quality 

### Overview

This project explores the relationship between various physicochemical properties of red wine and its quality, aiming to build a machine learning model for predicting wine quality based on its chemical features. The dataset consists of 1,143 records with 11 input features and a target variable indicating wine quality. The quality is rated on a scale from 3 to 8, where a higher number corresponds to better quality.

The project involves data exploration, feature engineering, handling class imbalance, and building models to predict wine quality.

### Objectives 

This data science project designed to:

- Analyze the physicochemical properties of wine (e.g., acidity, alcohol content, sugar levels) and their influence on wine quality.
- Build and evaluate machine learning models to predict wine quality.
- Address key challenges such as class imbalance and feature importance.
- Apply data preprocessing techniques to normalize features and improve model performance.

### EDA Questions

I want to answer the following questions:

1. What is the distribution of wine quality ratings across the dataset?
2. How do physicochemical properties relate to each other and to the wine quality?
3. What are the correlations between features, and how do these impact wine quality?

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

**Target Feature**:

- `quality`: Wine quality rating on a scale from 3 to 8

**Additional Column**:

- `Id`: Unique identifier for each record (not used for prediction)

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

7. **Model Building & Evaluation**
- Machine learning models, including Logistic Regression, Random Forest, and XGBoost, are trained and evaluated using various performance metrics, such as accuracy, precision, recall, and F1-score. The model's ability to handle class imbalance and predict rare quality classes is a critical focus.

8. **Visualization**
- Correlation heatmaps and distribution plots are created to visually understand the relationships between features and the target variable.

### Key Insights

- Most wines in the dataset have moderate levels of acidity, alcohol, and sugar, and quality scores are mostly in the middle range (around 5-6).
- Sulfur dioxide levels vary widely but are generally higher than the minimum, indicating the use of sulfur dioxide as a preservative in most wines.
- Alcohol content ranges between 8.4% and 14%, with most wines having alcohol levels between 9.5% and 11.1%.
- The model struggles with class imbalance, particularly for rare quality classes (e.g., 3, 4, 8), but performs better for more frequent classes like "5".
- The correlation between certain features reveals interesting relationships, such as a negative correlation between variables 0 and 8, suggesting an inverse relationship between these two features.

### Challenges & Future Work

- **Class Imbalance**: The model has difficulty predicting rare wine quality classes (e.g., 3, 4, 8). Future work should explore techniques like class weighting, undersampling, or more advanced resampling methods to improve performance for underrepresented classes.
- **Model Performance**: Further tuning of hyperparameters for models like XGBoost could improve prediction accuracy.
- **Feature Selection**: While PCA was used to reduce dimensionality, feature importance analysis could help identify the most impactful features for predicting wine quality.
- **Outliers & Feature Interactions**: Further exploration of outliers and the relationships between features can provide deeper insights into the data and model improvements.

### Future Improvements

- Implement hyperparameter tuning using grid search or random search for better model optimization.
- Use ensemble methods like Voting Classifier or Stacking to improve predictive power.
- Explore the impact of different resampling techniques to mitigate class imbalance more effectively.

### Source

Dataset: [Wine Quality Dataset on Kaggle](https://www.kaggle.com/datasets/yasserh/wine-quality-dataset)
