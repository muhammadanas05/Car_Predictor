# Car_Predictor
Machine Learning Project

# Used Car Price Prediction

This project focuses on predicting the prices of used cars based on various features such as the car's make, model, year of manufacture, kilometers driven, and fuel type. The prediction is done using machine learning techniques, primarily linear regression.

## Data Cleaning

The dataset used in this project contains information about various used cars. Before building the predictive model, it was essential to clean the data. The following steps were undertaken for data cleaning:

- Removal of non-numeric values from the 'year' column.
- Conversion of the 'year' column to integer data type.
- Removal of entries with "Ask for Price" in the 'Price' column.
- Conversion of the 'Price' column to integer data type.
- Extraction of numeric values from the 'kms_driven' column.
- Removal of NaN values from the 'fuel_type' column.
- Truncation of car names to the first three words.

The cleaned dataset was then saved as "Clean_Car_List.csv" for further analysis.

## Exploratory Data Analysis

Various visualizations were created to understand the relationship between different features and the price of the used cars:

- Box plot showing the relationship between the car's manufacturer and its price.
- Swarm plot illustrating the relationship between the manufacturing year and the price.
- Scatter plot depicting the relationship between kilometers driven and price.
- Box plot showing the relationship between fuel type and price.
- Scatter plot demonstrating the relationship between manufacturer, fuel type, manufacturing year, and price.

## Model Building

### Feature Extraction

The features used for model training include the name of the car, manufacturer, manufacturing year, kilometers driven, and fuel type.

### Train-Test Split

The dataset was split into training and testing sets using a 80:20 ratio.

### Preprocessing

One-hot encoding was performed on categorical features (car name, manufacturer, and fuel type) using sklearn's OneHotEncoder.

### Model Selection

Linear regression was chosen as the predictive model due to its simplicity and interpretability.

### Model Training and Evaluation

The pipeline consisting of data preprocessing and linear regression model was trained on the training data. The model's performance was evaluated using the R-squared metric on the testing data.

## Model Deployment

The best performing model was saved as "LinearRegressionModel.pkl" using pickle for future use. It can be utilized to predict the price of a used car given its features.

