### Overview: Insurance Claims Analysis

This project explores how health factors (blood pressure, BMI, diabetes, smoking), age, and gender impact insurance claim values. Initial exploratory data analysis (EDA) will utilize scatter plots, pie charts, and histograms to visualize relationships and distributions. Models will be built and evaluated to predict claim values, providing insights into risk assessment and policy pricing strategies.

### Steps
1. **Import Packages:** Import necessary libraries such as pandas, numpy, matplotlib, seaborn, plotly, scikit-learn components (Ridge, RandomForestRegressor, DecisionTreeRegressor), category_encoders, and ipywidgets.

2. **Import Dataset:** Load and set the dataset (`insurance_data.csv`).

3. **Data Inspection and Data Wrangling:**
   - Display the first few rows of data to understand its structure.
   - Check the shape and information of the dataset, including data types and missing values.
   - Perform data cleaning steps such as dropping missing values (NaN), handling duplicates, and removing columns with low cardinality or high multicollinearity.

4. **Data Visualization and Analysis:**
   - Visualize distributions and relationships using histograms, boxplots, violin plots, and pie charts to explore variables like age, BMI, blood pressure, and insurance claim values.
   - Analyze categorical variables such as gender, diabetic status, smoker status, and region.

5. **Data Modeling:**
   - **Baseline Model:** Establish a baseline using the mean value of insurance claims and calculate the Mean Absolute Error (MAE) as a benchmark.
   - **Machine Learning Models:**
     - **Ridge Regression:** Use Ridge regression with one-hot encoding for categorical variables.
     - **Random Forest Regressor:** Implement a Random Forest model for prediction.
     - **Decision Tree Regressor:** Employ a Decision Tree model for prediction.

6. **Model Evaluation:** Evaluate each model's performance using Mean Absolute Error (MAE).

7. **Prediction Function:** Create a function (`make_prediction`) to make predictions based on the inputs for age, gender, BMI, blood pressure, diabetic status, number of children, smoker status, and region.

8. **Interactive Prediction:** Utilize ipywidgets to create an interactive interface where users can input their data and get a predicted insurance claim value based on the Decision Tree model.
