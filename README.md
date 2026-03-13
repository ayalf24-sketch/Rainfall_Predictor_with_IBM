# Rainfall_Predictor_with_IBM

Rainfall Prediction – Machine Learning Project (Python)

This project predicts whether it will rain today using historical weather data from multiple locations in Melbourne, Australia. The project leverages machine learning pipelines, feature engineering, and model evaluation techniques. It was completed as a final project in an IBM Machine Learning course.

**Features**

**Data Preprocessing:**

Reads CSV weather data from an online source.

Cleans missing values and selects relevant locations (Melbourne, Melbourne Airport, Watsonia).

Converts dates into seasons (Summer, Autumn, Winter, Spring) for additional features.

Differentiates between numeric and categorical variables.

**Machine Learning Pipelines:**

Uses ColumnTransformer for preprocessing numeric and categorical features:

Numeric features → Standard Scaler

Categorical features → One-Hot Encoding

Integrates preprocessing and classification into a single Pipeline.

**Models Implemented:**

Random Forest Classifier

Hyperparameter tuning using GridSearchCV and StratifiedKFold cross-validation.

Feature importance analysis to identify top predictors of rainfall.

Logistic Regression

Evaluates model performance with different solvers, penalties, and class weights.

**Evaluation:**

Accuracy and classification reports on train and test sets.

Confusion matrices visualized with matplotlib and seaborn.

Feature importance is plotted to understand the key drivers of rainfall.

**Implementation Highlights**

Top Features for Rain Prediction:
The project identifies the most important features influencing rainfall, such as temperature, humidity, wind direction, and past rainfall.

Cross-Validation & Grid Search:
Ensures robust model selection and prevents overfitting by tuning hyperparameters.

**Visualization:**

Confusion matrices for both classifiers.

Horizontal bar chart of the top N most important features.

**Usage**
The pipeline automatically handles preprocessing and classification.

Outputs include:

Best hyperparameters for each model

Cross-validation and test set accuracy

Classification report (precision, recall, F1-score)

Confusion matrix

Feature importance visualization

**Technologies Used**

Pandas and NumPy for data manipulation

scikit-learn for machine learning

Matplotlib and Seaborn for visualization

**Results**

Random Forest generally achieves higher accuracy and provides insight into key features.

Logistic Regression offers a simpler, interpretable baseline model.
