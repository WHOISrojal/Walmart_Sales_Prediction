# Walmart Sales Prediction

Walmart Sales Prediction is the strategic use of data analysis, statistical modeling, and machine learning techniques to forecast and anticipate future sales trends and patterns within Walmart's retail ecosystem, one of the world's largest and most influential retail chains.


## Linear equation flow for Walmart Sales Prediction:

1. Necessary data import
2. Data load
3. EDA
	i. Null-values check (rename/fill)
	ii. Duplicated Rows (remove)
4. Feature Engineering (To know Importance)	
5. Split into independent and dependent features (x, y)
6. Train-Test Split (x_train, x_test, y_train, y_test)
7. Create object of class (Class of algorithm)
8. Fit the data into algorithm (. fit ())
9. Check the matrices (Accuracy / Errors)

## Project Structure

The project is organized as follows:

1. Data Preprocessing
Loading Data: The dataset is loaded using pandas from a CSV file.
Null Value Check: Ensures that there are no missing values in the dataset.
Duplicate Data Check: Identifies and removes any duplicate rows in the dataset.
Unique Data Check: Checks the uniqueness of the data in certain columns.
2. Exploratory Data Analysis (EDA)
Descriptive Statistics: Provides a summary of the data including count, mean, standard deviation, and other statistical metrics.
Data Types and Information: Displays the data types of each column and provides information about memory usage.
Correlation Analysis: Computes and visualizes the correlation matrix to identify relationships between different features.
3. Feature Engineering
Date Encoding: The Date column is converted into a numerical format using Label Encoding.
Datetime Features: Extracts additional features such as year, month, day of the week, and quarter from the Date column.
Season Classification: Classifies dates into seasons based on specific date ranges.
Target Guided Encoding: Encodes categorical variables such as day, month, and year based on their relationship with the target variable, Weekly_Sales.
Categorical to Dummy Variables: Converts categorical variables into dummy/indicator variables for use in the model.
4. Data Visualization
Histograms: Visualizes the distribution of all features in the dataset.
Correlation Heatmap: A heatmap to visualize the correlations between different features.
5. Model Training and Evaluation
Feature Scaling: Standardizes the features using StandardScaler to ensure all features contribute equally to the model.
Train-Test Split: Splits the dataset into training (70%) and testing (30%) sets.
Linear Regression Model: A linear regression model is trained on the training data.
Model Evaluation: The model is evaluated using Mean Squared Error (MSE), Mean Absolute Error (MAE), and R-Squared (R²) score.
6. Results
Predicted vs Actual Sales: The predictions are compared with the actual sales to assess the model's performance.
Regression Line Plot: Visualizes the relationship between predicted and actual sales on both training and testing datasets.
7. Model Deployment
Model Saving: The trained model is saved using pickle for future use in deployment

## Installation
To run this project, you need to have the following dependencies installed:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- pickle
  
You can install these dependencies using pip:
```
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Usage
1. Clone the repository:
```
git clone https://github.com/yourusername/walmart-sales-prediction.git
cd walmart-sales-prediction
```

2. Run the main script:
```
python main.py
```

3.View the results and visualizations in your terminal or output files.
