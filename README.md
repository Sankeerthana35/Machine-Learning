1. Data Loading & Exploration
The dataset (CarPrice_Assignment.csv) is loaded into a DataFrame. Basic exploration is performed, including checking column types, missing values, and overall data structure. This helps in understanding the dataset before applying any transformations.

2. Data Preprocessing
Dropping Unnecessary Columns: The car_ID column is removed since it is just an identifier and does not contribute to price prediction.
Handling Categorical Variables: Since machine learning models require numerical inputs, categorical features (like fuel type and car body) are converted into numerical values using one-hot encoding.
Feature Selection: The target variable (price) is separated from the features (X).
3. Splitting Data for Training and Testing
The dataset is split into training (80%) and testing (20%) subsets. The training data is used to develop the model, while the test data is reserved to evaluate its performance on unseen data.

4. Feature Scaling
Since the dataset contains features with different scales (e.g., horsepower in hundreds, compression ratio in single digits), standardization is applied to ensure all features contribute equally. This improves the performance of models like linear regression and gradient boosting.

5. Model Training & Selection
The notebook includes multiple regression models:

Linear Regression – A simple model assuming a direct relationship between features and price.
Decision Tree Regression – A tree-based model that splits data into rules for better prediction.
Random Forest Regression – An ensemble method using multiple decision trees for more accurate results.
Gradient Boosting Regression – A powerful boosting technique that builds models sequentially, improving performance over time.
Each model is trained on the scaled training data.

6. Model Evaluation
The trained models are tested on the unseen data, and performance metrics like R² score, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE) are used to compare their accuracy.
