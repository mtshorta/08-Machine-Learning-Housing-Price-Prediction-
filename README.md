# São Paulo Housing Price Prediction with Machine Learning

This project focuses on utilizing machine learning techniques for predicting housing prices in São Paulo, Brazil, using machine learning techniques. 
The analysis and predictions are based on historical housing transaction data provided in a CSV file available in Kaggle:
https://www.kaggle.com/datasets/argonalyst/sao-paulo-real-estate-sale-rent-april-2019

Context
The dataset represents properties advertised in the month of April 2019.
This dataset contains around 13.000 apartments for sale and for rent in the city of São Paulo, Brazil. 
The data comes from multiple sources, specially real estate classified websites.


## Project Overview

This project involves the following steps:

1. **Data Ingestion**: 
   - We start by loading a CSV file containing housing listings data in São Paulo in april 2019.
   - The data is converted into a pandas DataFrame for easier manipulation and analysis.

2. **Exploratory Data Analysis (EDA)**:
   - We perform an exploratory data analysis to understand the distribution of housing prices, identify trends, and detect any potential outliers.
   - Various visualizations and statistical summaries are generated to guide further analysis.

3. **Data Cleaning**:
   - The dataset is cleaned to remove or correct any missing, inconsistent, or irrelevant data.
   - We handle issues such as missing values, incorrect data types, and duplicated entries to ensure the quality of the data.

4. **Geospatial Visualization**:
   - Using the Mapbox API, we plot a geospatial graph to visualize the relationship between property prices and their sizes across different regions of São Paulo.
   - This helps in identifying geographical trends and price clusters within the city.

5. **Model Training**:
   - We train three different machine learning models to predict housing prices:
     - **Decision Tree**
     - **Random Forest**
     - **Linear Regression**
   - These models are trained on the cleaned dataset and evaluated for performance.

6. **Model Comparison**:
   - We use cross-validation to compare the performance of the three models.
   - Based on the cross-validation results, we determine that the **Random Forest** model performs the best on this dataset.

7. **Model Optimization**:
   - The Random Forest model is further optimized using GridSearch to fine-tune hyperparameters and improve accuracy.

8. **Prediction Visualization**:
   - Finally, we plot a graph comparing the predicted housing prices against the actual prices from the dataset.
   - This visualization provides insights into the model's accuracy and highlights any discrepancies between predicted and actual values.

## Requirements
- pandas
- plotly.express
- plotly.graph_objects
- matplotlib.pyplot
- seaborn
- numpy
- sklearn
